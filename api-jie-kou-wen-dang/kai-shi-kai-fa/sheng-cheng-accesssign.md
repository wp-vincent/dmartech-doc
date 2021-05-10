# 接口签名生成说明

**签名生成说明**

* 获得现在的毫秒时间戳
* 将时间戳用access-secret进行AES加密,获得加密后字符串
* 将字符串用base64进行转码,再用UTF-8编码获得签名
* 用来加密的时间戳不能与现在时间相差超过5分钟

java代码示例

```text
    /** 算法 */
    private static final String ALGORITHM = "AES/ECB/PKCS5Padding";

    /**
     * AES加密字符串
     *
     * @param content  需要被加密的字符串
     * @param password 加密需要的密码
     * @return 密文
     */
    public static String encrypt(String content, String password) {
        try {
            // 转换为AES专用密钥
            SecretKeySpec key = new SecretKeySpec(password.getBytes(), "AES");
            // 创建密码器
            Cipher cipher = Cipher.getInstance(ALGORITHM);
            // 初始化为加密模式的密码器
            cipher.init(Cipher.ENCRYPT_MODE, key);
            byte[] byteContent = content.getBytes("UTF-8");
            // 加密
            byte[] result = cipher.doFinal(byteContent);
            //转换加密后产生的特殊字符，比如"+"
            String accessKeySecret = Base64.encodeBase64String(result);
            try {
                accessKeySecret = URLEncoder.encode(accessKeySecret, "UTF-8");
            } catch (UnsupportedEncodingException e) {
                log.error(String.format("AES加密异常, content: %s, password: %s, err: %s", content, password, e));
            }
            return accessKeySecret;
        } catch (Exception e) {
            log.error(String.format("AES加密异常, content: $s, password: $s, err: $s", content, password, e));
            return null;
        }

    }
```

**java SDK**

{% file src="../../.gitbook/assets/openapisdk.zip" %}


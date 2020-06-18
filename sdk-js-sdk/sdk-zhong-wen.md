---
description: SDK中文接口文档
---

# SDK（中文）

## 下载SDK

请登录Dmartech平台，从“数据中心”-“数据中心”，点击”数据接入“进入，找到”服务器端接入 SDK“得到SDK

## 环境配置

### **1.添加依赖Fastjson**

```text
 <dependency>

    <groupId>com.alibaba</groupId>

    <artifactId>fastjson</artifactId>

    <version>1.2.31</version>

</dependency>
```

### **2.将下载的jar包放到项目lib目录下**

```text
/src/main/resources/lib
```

### **3.配置pom.xml**

```text
<dependency>

   <groupId>com.qdum</groupId>

   <artifactId>sdk</artifactId>

   <version>1.0</version>

   <scope>system</scope>

   <systemPath>${project.basedir}/src/main/resources/lib/java_sdk.jar</systemPath>

</dependency>
```

## SDK接口

### 接口分类

| 接口类别 | 接口名 | 参数列表 |
| :--- | :--- | :--- |
| 用户数据接口 | user | 用户属性 |
| 删除用户接口 | userDelete | 带主键标识的用户属性 |
| 事件数据接口 | event | 事件名, 带主键标识的用户属性及该事件关联的事件属性 |

### 参数说明

  
properties中都需要"带主键标识的用户属性"且至少一个有值.

特别说明: 1. "带主键标识的用户属性": 在"数据中心-元数据-用户属性"中可以将某些属性设置为主键标识, 例如将手机号和邮箱设为主键标识, 在导入数据时会根据这两个属性查询用户并更新数据  
2. 事件数据接口中需要两个额外的属性,"event\_id"和"create\_time",event\_id为该事件数据的唯一标识,create\_time为该事件发生的时间.

## 使用SDK

### 用户数据示例

```text
// 声明SDK对象, 需要SECRET
 
JavaSdk sdk = new JavaSdk(" 1d220cf5-4237-491e-8f05-0c2190adxxxx");
 
 
// 调试模式:只校验格式不执行入库. 注意:默认值为false, 生产环境务必将此参数设置为false或注释掉该配置.
 
sdk.setDebug(true);
```

```text
/* 导入用户示例 开始 */
 
JSONObject properties = new JSONObject();
 
 
// phone, email 为主键标识的用户属性
 
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// username, age 为普通的用户属性
 
properties.put("username", "tianshl");
 
properties.put("age", 80);
 
 
// 发送请求
 
String response = sdk.user(properties);
 
// 输出结果
 
System.out.println(response);
 
/* 导入用户示例 结束 */
```

### 事件数据示例

```text
// 声明SDK对象, 需要SECRET
 
JavaSdk sdk = new JavaSdk(" 1d220cf5-4237-491e-8f05-0c2190adxxxx");
 
 
// 调试模式:只校验格式不执行入库. 注意:默认值为false, 生产环境务必将此参数设置为false或注释掉该配置.
 
sdk.setDebug(true);
```

```text
/* 导入事件示例 开始 */
 
JSONObject properties = new JSONObject();
 
 
// phone, email 为主键标识的用户属性
 
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// orderId, orderTime, amount 为事件属性
 
properties.put("orderId", "20180808080800001");
 
properties.put("orderTime", "2018-08-08 08:08:08");
 
properties.put("amount", 998);
 
 
// eventId, create_time 为额外的参数
 
properties.put("event_id", "20180808080800001");
 
properties.put("create_time", "2018-08-08 08:08:08");
 
 
// 发送请求
 
String response = sdk.event("orderDetail", properties);
 
// 输出结果
 
System.out.println(response);
 
/* 导入事件示例 结束 */
```

### 删除用户示例

```text
// 声明SDK对象, 需要SECRET
 
JavaSdk sdk = new JavaSdk(" 1d220cf5-4237-491e-8f05-0c2190adxxxx");
 
 
// 调试模式:只校验格式不执行入库. 注意:默认值为false, 生产环境务必将此参数设置为false或注释掉该配置.
 
sdk.setDebug(true);
```

```text
/* 删除用户示例 开始 */
 
JSONObject properties = new JSONObject();
 
 
// phone, email 为主键标识的用户属性
 
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// 发送请求
 
String response = sdk.userDelete(properties);
 
// 输出结果
 
System.out.println(response);
 
/* 删除用户示例 结束 */
```

### 返回结果

#### 正确时的返回JSON包如下 

{"errcode":0,"errmsg":"请求成功"}  


#### 错误时的返回JSON包如下 

{"errcode":10001,"errmsg":"json数据格式化失败"}  


### 返回码说明

| 返回码 | 说明 |
| :--- | :--- |
| 0 | 请求成功 |
| 10000 | 系统错误 |
| 10001 | json数据格式化失败 |
| 10002 | type取值不合法 |
| 10003 | 缺少secret参数 |
| 10004 | 属性列表为空 |
| 20000 | 身份验证失败 |
| 20001 | 缺少主键标识的用户属性 |
| 20002 | 至少需要一个主键标识的用户属性存在值 |
| 20003 | 数据校验失败 |

### 备注

该结果只是标识请求结果, 数据导入结果请查看系统中相关数据源的导入详情


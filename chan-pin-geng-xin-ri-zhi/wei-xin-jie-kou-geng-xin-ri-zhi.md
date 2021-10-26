# 微信接口更新日志

### 2021-10-20 微信接口调整

根据最新法规，微信于2021-10月20日调整了用户信息相关接口和功能。详情请见：[https://developers.weixin.qq.com/community/develop/doc/00028edbe3c58081e7cc834705b801](https://developers.weixin.qq.com/community/develop/doc/00028edbe3c58081e7cc834705b801)

鉴于上述公告及国家最新隐私政策法规，Dmartech将于近期下线相关功能：

* 微信管理-粉丝管理：筛选器中将不再提供“性别“、“地区“、“语言“的选项。
* 微信管理-自定义菜单-个性化菜单：筛选条件中将不再提供“性别“、“地区“、“语言“的选项。已经设置好的规则，将从中移除掉“性别“、“地区“、“语言“的筛选条件。
* 元数据：将从用户属性中移除：“language\_wechat“, "province\_wechat", "country\_wechat", "city\_wechat", "sex\_wechat" 共计5个属性字段。
* 元数据中移除这些字段后，将无法在联系人分群、旅程中的条件分支等涉及分群筛选的功能中继续使用。页无法在插入自定义字段的地方使用。




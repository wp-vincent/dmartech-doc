---
description: JS-SDK Interface（English）
---

# JS-SDK（English）

## **Download SDK**

  
 Please log in to the Dmartech，from the "Data Center" - "Data Center", click on "Data Access" to enter，find the "Client access SDK" to get the JS-SDK

## **SDK** Interface

### Interface **category**

| Interface **category** | Interface name | parameter list |
| :--- | :--- | :--- |
| user data nterface | user | properties，callback |
| Delete user nterface | userDelete | properties，callback |
| Event data nterface | event | eventName，properties，callback |

| parameter name | parameter |
| :--- | :--- |
| properties | Attribute list |
| eventName | Event name |
| callback | callback function |

### **Parameter description**

Properties must be user properties whose are primary key and at least has one valid value.

Special tips:

1.Properties’ primary key attributes can be set at data center àmeta dataàcustomer properties.

2.Event interface needs two extra properties, “event\_id”  and “create\_time”, “event\_id” is primary key of that event and create\_time is the time of this event.  
 

### **How to use** **SDK**

#### **customer data example**

```text
// create SDK object, SECRET needed here
var sdk = new this.SDK("daccb41a-5cfb-42d1-8bee-32aa0156xxxx");

// debub mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
sdk.setDebug(true);
```

```text
/* import customer example begin */
 
// phone, email are customer properties whose attributes are primary key.
 
// username, age are ordinary customer properties.

var properties = {
 
"phone": "183****6527",
 
"email": "tianshl@qdum.com",
 
"username": "tianshl",
 
"age": 80
 
};

 // send request）
 
sdk.user(properties, function(resp){
 
// this is the callback method
 
console.log(resp);
 
});
 
/* import customer end */
```

#### **Event data example**

```text
// create new SDK object, SECRET needed
var sdk = new this.SDK("daccb41a-5cfb-42d1-8bee-32aa0156xxxx");

// debug mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
sdk.setDebug(true);
```

```text
/* import event data begin */ 

// phone, email are customer properties whose attributes are primary key. 
 
// orderId, orderTime, amount are event properties
 
// eventId, create_time are extra properties
 
var properties = {
 
"phone": "183****6527",
 
"email": "tianshl@qdum.com",
 
"orderId": "20180808080800001",
 
"orderTime": "2018-08-08 08:08:08",
 
"amount": 998,
 
"event_id": "20180808080800001",
 
"create_time": "2018-08-08 08:08:08"
 
};

 
// send request
 
sdk.event("order_detail", properties, function(resp){
 
// this is the callback method
 
console.log(resp);
 
});
 
/* event import example end */
```

#### **Delete customer data example**

```text
// create new SDK object,  SECRET needed
var sdk = new this.SDK("daccb41a-5cfb-42d1-8bee-32aa0156xxxx");

// debug mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
sdk.setDebug(true);
```

```text
/* delete customer data example begin */
 
// phone, email are customer properties whose attributes are primary key. 
 
var properties = {
 
"phone": "183****6527",
 
"email": "tianshl@qdum.com"
 
};

 // send request
 
sdk.userDelete(properties, function(resp){
 
// this is the callback method
 
console.log(resp);
 
})
 
/* delete customer data example end */
```

#### **output**

**successful** **JSON** **return**

{"errcode":0,"errmsg":"请求成功"}

**Error JSON return**

{"errcode":10001,"errmsg":"json数据格式化失败"}

#### **Return code descriptons**

| Return code | description |
| :--- | :--- |
| 0 | successful |
| 10000 | system error |
| 10001 | Json deta formatting failed |
| 10002 | invalid type value |
| 10003 | Secret parameters required |
| 10004 | Properties are empty |
| 20000 | Authentication failed |
| 20001 | Lack of property which is primary key |
| 20002 | At least one valid value is needed in property which is primary key |
| 20003 | Data checking failed |
| 20004 | Signature checking failed |

#### **Tips**

The result is only to identify the result of the request. For the data import result, please check the import details of the relevant data source in the system.


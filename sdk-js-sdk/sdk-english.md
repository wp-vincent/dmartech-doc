---
description: SDK Interface
---

# SDK（English）

## **Download SDK** 

Please log in to the Dmartech，from the "Data Center" - "Data Center", click on "Data Access" to enter，find the "Sever access SDK" to get the SDK

## **Environment Setup**

### **1.adding dependency** **Fastjson**

```text
<dependency>

  <groupId>com.alibaba</groupId>

  <artifactId>fastjson</artifactId>

  <version>1.2.31</version>

</dependency>
```

### **2. put downloaded jar file to path below**

```text
/src/main/resources/lib
```

### **3.config pom.xml**

```text
<dependency>

   <groupId>com.qdum</groupId>

   <artifactId>sdk</artifactId>

   <version>1.0</version>

   <scope>system</scope>

   <systemPath>${project.basedir}/src/main/resources/lib/java_sdk.jar</systemPath>

</dependency>
```

## **SDK interface**

### **Interface category**

| Interface category | Interface   Name | parameters |
| :--- | :--- | :--- |
| customer data interface | customer | customer properties |
| Delete customer data interface | userDelete | customer properties whose are primary key attributes |
| Event data interface | event | Event name, customer properties whose are key attributes and event related properties  |

### **Parameters description**

Properties must be user properties whose are primary key and at least has one valid value.

Special tips:

1.Properties’ primary key attributes can be set at data center àmeta dataàcustomer properties.

2.Event interface needs two extra properties, “event\_id”  and “create\_time”, “event\_id” is primary key of that event and create\_time is the time of this event.  


## **How to use** **SDK**

### **customer data example**

```text
// create SDK object, SECRET needed here
JavaSdk sdk = new JavaSdk(" 9db51757-8b33-496a-895c-0ecf2b79xxxx ");

// debub mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
sdk.setDebug(true);
```

```text
/* import customer example begin */
 
JSONObject properties = new JSONObject();
 
 
// phone, email are customer properties whose attributes are primary key.
 
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// username, age are ordinary customer properties.
 
properties.put("username", "tianshl");
 
properties.put("age", 80);
 
 
// send request
 
String response = sdk.user(properties);
 
// output
 
System.out.println(response);
 
/* import customer end */
```

### **Event data example**

```text
// create new SDK object, SECRET needed
 
JavaSdk sdk = new JavaSdk(" 9db51757-8b33-496a-895c-0ecf2b79XXXX");
 
 
// debug mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
 
sdk.setDebug(true);
```

```text
/* import event data begin */
 
JSONObject properties = new JSONObject();
 
 
// phone, email are customer properties whose attributes are primary key. 
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// orderId, orderTime, amount are event properties
 
properties.put("orderId", "20180808080800001");
 
properties.put("orderTime", "2018-08-08 08:08:08");
 
properties.put("amount", 998);
 
 
// eventId, create_time are extra properties
 
properties.put("event_id", "20180808080800001");
 
properties.put("create_time", "2018-08-08 08:08:08");
 
 
// send request
 
String response = sdk.event("orderDetail", properties);
 
// output
 
System.out.println(response);
 
/* event import example end */
```

### **Delete customer data example**

```text
// create new SDK object,  SECRET needed
JavaSdk sdk = new JavaSdk(" 9db51757-8b33-496a-895c-0ecf2b79xxxx ");

// debug mode:only check format, not importing the data. Tips: default value is false, set this value to false or comment off this setting in production environment
sdk.setDebug(true);
```

```text
/* delete customer data example begin */
 
JSONObject properties = new JSONObject();
 
 
// phone, email are customer properties whose attributes are primary key.  
properties.put("phone", "183****6527");
 
properties.put("email", "tianshl@qdum.com");
 
 
// send request
 
String response = sdk.userDelete(properties);
 
// output
 
System.out.println(response);
 
/* delete customer data example end */
```

### **output**

**successful** **JSON** **return**

{"errcode":0,"errmsg":"请求成功"}

**Error JSON return**

{"errcode":10001,"errmsg":" json数据格式化失败"}

### **Return code descriptons**

| Return code | description |
| :--- | :--- |
| 0 | Successful |
| 1000 | System error |
| 10001 | Json data formatting failed |
| 10002 | Invalid type value |
| 10003 | Secret parameters required |
| 10004 | Properties are empty |
| 20000 | Authentication failed |
| 20001 | Lack of property which is primary key |
| 20002 | At least one valid value is needed in property which is primary key |
| 20003 | Data checking failed |

### **Tips**

The result is only to identify the result of the request. For the data import result, please check the import details of the relevant data source in the system.


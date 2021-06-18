# Mass message

Three types of WeChat messages are supported: mass messages, customer service messages, and template messages.

For the latest rules on sending messages, please see the official description of WeChat: [https://developers.weixin.qq.com/doc/offiaccount/Message\_Management/Batch\_Sends\_and\_Originality\_Checks.html](https://developers.weixin.qq.com/doc/offiaccount/Message_Management/Batch_Sends_and_Originality_Checks.html)

### **1. Mass messaging**

For the authentication service number, although the developer can use the advanced mass sending interface to call 100 times per day, the user can only receive 4 messages per month. No matter on the public platform website or using the interface to mass send, the user can only receive 4 messages per month. If the user sends more than 4 messages, the user will fail to send to the user.

For the authenticated subscription number, the mass send interface can be successfully called once a day. This time, the mass send can be sent to all users or a label.

![](../.gitbook/assets/image%20%2846%29.gif)

1\) Mass Sends: All fans or fans under a certain tag can be selected. For details of fans and fan tags, see "Fan Management";

2\) Send type: can be sent immediately or timed;

3\) Select material: support to send text message, text, pictures, audio, video, send material can be created from the "material management" to select the corresponding material, can be new;

4\) Click the "Send" button to execute the message and send the command;

5\) Click "Sent" to enter the page of historical sending records to view the historical sending situation;

**2.customer service news**

Only sent to fans who have had any of the following interactions within 48 hours, meaning:

* User Sends Message
* Click the custom menu \(the customer service interface will be triggered only by clicking the three menu types: push event, scan push event, scan push event and pop up the prompt box of "message receiving"\)
* Follow the public account
* Scan QR code
* Pay for success
* The user rights

![](../.gitbook/assets/image%20%2844%29.gif)

3. Template messages

1\) All service numbers can see the entrance of application template message function in the WeChat public background "Functions -&gt; Add Functions" plug-in, but only authenticated service numbers can apply for the permission to use template messages and get the permission;

2\) You need to choose the two industries in which the public account service is located, and you can change the selected industry once a month;

3\) Select the existing template from the template library of the selected industry to make the call;

4\) Each account can use 25 templates at the same time.

5\) Currently, the daily call limit of each account's template message is 100,000 times, and there is no special limit for a single template. \[On November 18, 2014, the frequency of interface calls was increased from the default 10,000 times per day to 100,000 times per day, which can be viewed in the Developer Center after MP login\]. When the number of followers of the account exceeds 10W/100W/1000W, the daily call limit of the template message will be increased accordingly, and the number indicated in the developer center page of the public account MP background shall prevail.

DMARTECH opens the function of actively sending template messages to fans, in order to better help customers maintain fans. But do not abuse this function, a large number of template messages will lead to fan complaints, your public account will be warned or closed. DMARTech assumes no responsibility and cannot promise or guarantee the arrival rate or complaint rate.

![](../.gitbook/assets/image%20%2849%29.gif)

### Sent

You can view the sending records of various kinds of messages and see the actual sending status.

![](../.gitbook/assets/image%20%2851%29.gif)












































































# Appendix 4 Quickly Understand the Marketing Journey

### Take the e-commerce user life cycle as an example 

The figure below shows a simple and common e-commerce user life cycle. After entering the product, users go through five stages.

![](.gitbook/assets/image%20%28532%29.png)

#### Common problems 

1.The user who has visited our website is a real user.

 In fact, this is not the case. The real user is somebody who has completed a core process of the product at least once. That is, a real user has completed a closed-loop purchase for the e-commerce, and it is active currently. 

2.As long as the user who has passed the novice period will not leave our product. 

Users can abandon the product at any time as long as they find that the product is not helpful to them, so we need to let all users concentrate to the maturity stage. 

3.Users will come to buy as long as we recommend the high-quality goods in the product to them. 

In fact, users just care about what they really need, but not popular. 

4.Lost users will not come back to use the product again. 

If the marketing is done well, and the products are indeed required for the lost users, they will come back to buy it when they need. Furthermore, the conversion cost of attracting a new user is more than 10 times than recalling the lost users. So, it is necessary to recall the lost users.

### Solution 

1.Establishing automated marketing for potential users, and letting them enter the novice stage. You can tag potential customers who have registered but not placed an order yet by using Dmartech’s automated marketing function. This function supports to send marketing content regularly through different channels. In Dmartech, you can also know whether the user is finally activated to place an order.

![](.gitbook/assets/image%20%28560%29.png)

2.Pushing personalized emails contained products that users may be interested in. Recommend similar products based on the product that the user opens the link in the email.

![](.gitbook/assets/image%20%28505%29.png)

3.Building a user lifecycle journey, tagging users who meet the filter criteria, and glancing what stages are all users in quickly. You can view the current lifecycle, habits, historical behavior and consumption history of each user. Combining personalized emails mentioned in the previous step for different users to refine the operation of users.

![](.gitbook/assets/image%20%28548%29.png)

### Conference process automation 

**1.Background** 

Inviting existing customers to attend the conference. 

**2.Purpose** 

Collecting customer information to improve customer portraits. Obtaining more information for later use. 

**3.Difficulties** 

The meeting takes a long time from preparation to completion, and the labor cost is too large. The collected information cannot be associated with the customer, or the association takes a long time. So it is unable to connect customers' information in different channels. 

**4.Analysis method** 

Dividing the meeting task into three stages: registration - sign in – end. We can determine the data can be collected at each stage and let the process run automatically. 

**5.Scheme**

 Establish a fully automated conference process, including registration, sign in, and end stages. The conference process also can be divided into multiple stages. Here is an example of a process.

### Advantage 

The conference can be proceed automatically through the program. Dmartech can realize to collect user information within a reasonable period of time and will not arouse disgust. After the data is cleaned internally by Dmartech, the platform will finally open up all user data to realize the construction of user portraits.

![](.gitbook/assets/image%20%28568%29.png)

**Step 1 Registration stage** 

1.Determine when to start — start setting 

a.Create the form and QR code in QR code mgt and Form page first. 

b.Audience grouping: No restriction. 

c.Trigger conditions: Contact Activity \(WeChat event – scan QR code with parameters – official account – QR code name.

![](.gitbook/assets/image%20%28549%29.png)

2.Template message — notify users

 After scanning the code, a template message will be pushed to the user in the official account, and the user can click the template to register.

![](.gitbook/assets/image%20%28515%29.png)

3.Event Condition — judge whether the user opens the form

 Event condition can judge whether the users who scanned the code have opened the form.

![](.gitbook/assets/image%20%28553%29.png)

4.Add tags

 If the user does not open the form, these users can be tagged as Not open. 

5.Event Condition — judge whether to submit the registration form

 If the user submits the form, we can collect part of the user's information through the form.

![](.gitbook/assets/image%20%28492%29.png)

6.Add tags 

If the user does not submit the form, we can also tag this part of the user as Open uncommitted. 

7.Add tags

 If the user submits the form, we need to tag it as Sigh up to provide reference for future sign-in. 

8.SMS reminder 

Automatically send SMS to remind users the day before the conference. The above is the construction process and rules of the registration stage during the whole journey of the conference.

![](.gitbook/assets/image%20%28561%29.png)

**Step 2 Sign-in stage** 

1.Event Condition — judge whether to submit the registration form 

When the conference starts to sign in, users can scan the QR code to sign in. 

2.Add tags — determine the number of people who sign in by scanning the code

 All users who have scanned the code will be signed in by default and will be marked with the tag Checked in. And the users who have not scanned the code will be marked with the tag Not checked in. 

3.Template message —sign-in success notification 

After the user scans the QR code, the sign-in is successful. The user is notified by sending a WeChat template message. 

The above is the construction process and rules of the sign-in stage during the whole journey of the conference.

**Step 3 End stage** 

1.Event Condition — obtain information After the conference, the user scans the new QR code to fill in the email address to get the conference document.

![](.gitbook/assets/image%20%28495%29.png)

2.Add tags — determine the number of people who have scanned the code

 Mark users who have not submitted the form as unsubmitted and users who have submitted the form as submitted. 

3.Send email 

Send an email with conference documents to users.

![](.gitbook/assets/image%20%28490%29.png)

The full-process case of the conference built through the marketing journey can collect information according to the content of the activity without the user's perception, which is conducive to us building user portraits.


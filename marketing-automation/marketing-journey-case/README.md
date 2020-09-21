# Marketing Journey Case

We use a case here for reference in order to facilitate you to better understand and use with Dmartech.

### Background

A SaaS software supplier planned a series of marketing plans including product advertising, new customer operation, potential user incubation, and old customer retention. 

It will cost immense manpower and material resource to use traditional manual follow-up methods as well as an information transmission lag. 

However, using Dmartech to automate the marketing journey can easily realize the plan. 

* The case of a single time journey 

Based on the company's existing customer data, you can send marketing mailings, short messages through a single time journey. You can also send graphic messages to followers who have followed the WeChat official account. The contents for each channel can be daily marketing contents such as product introduction, corporate dynamic introduction and preferential activities. You can push them to the contacts at any time at once by using Dmartech.

### Journey Settings

a.Select the segment to be sent, the multiple segments also can be selected. As the figure shows below, segment1 and segment2 have been selected. 

b.Judge whether the contacts in the selected segment has a value in their WeChat unionid field. If yes, a WeChat graphic message will be sent out. If no, continue to judge whether the email field has a value. Then send an email or send a short message according to the result.

![](../../.gitbook/assets/image%20%28524%29.png)

The general usage scenario of a single journey is that all the contacts in the specified segment will enter the journey at the same time. You can set filter criteria according to attribute or event to send marketing contents to qualified contacts. Of course, you can also directly send marketing contents to contacts in the specified segment.

* The case of a real-time journey 

New user welcome journey 

Users can fill in the form on the official website to register for the product trial. In order for new users to have a good service experience, we should send a welcome email to registered users as soon as the registration is successful. The product trial expires in 7 days and we need to remind users to buy official products before expiration. Judge whether the user has placed an order to purchase after registering for the trial. If the order is placed, it will be tagged as first order, if the order has not been placed, it will be marked as trial not placed. 

Two events are involved: registration and order placement. These two events are not Dmartech's system preset events, so you need to define register event in Meta data &gt; Event management/ Event properties, and then import the event into Dmartech through an interface to use the event. Users who have registered events will trigger a real-time journey named welcome new users.

### Journey Settings 

a.Trigger event: user registration. 

b.Send a welcome email to the contacts who has entered the journey. 

c.Send expiration and purchase reminder emails to the contacts after 6 days. 

d.Judge whether the trial user has placed an order. If the order is placed, tag the contact as first order; if the order is not placed, tag the contact as trial not placed.

![](../../.gitbook/assets/image%20%28525%29.png)

* Clue incubation journey 

For trial users who have not placed an order, it is a clue that enterprises need to focus on incubation and promotion. Send the emails about the advantages and highlights of the product to these users, and continue to judge whether to place an order. If the order is placed, tag the contact as first order; if not, send a promotional email or issue a coupon, and continue to judge whether to place an order. If yes, tag the contact as first order; if not, tag the contact as not hatched. 

### Journey Settings 

a.Set the real-time journey trigger to contacts who has been tagged as trial not placed enter the journey. 

b.Send product advantages and highlights introduction emails. 

c.Judge whether to place an order. If yes, tag the contact as first order; if not, send a promotional email. 

d.Continue to judge whether to place an order. If yes, tag the contact as first order; if not, tag the contact as not hatched.

![](../../.gitbook/assets/image%20%28538%29.png)

* Maintain old customers journey 

In order to better serve customers, promote contract renewal, and let the new users become a long-term customer, we need to send the satisfaction survey form to the customer since the new user formally uses the product 30 days later. Then respond the Thanks email immediately after receiving the form submission. Reply the corresponding email immediately in response to the different content submitted by the customer.

![](../../.gitbook/assets/image%20%28509%29.png)


# View the Journey Report

You can view and download reports related to marketing journeys and channels in Campaign report module. Choose Data center &gt; Campaign report from the main menu to enter the Journey report review page, which includes three tab pages: Automation overview, Messages list, Export Data.

**View the Report of All Journeys or Specified Journeys within a Certain Period of Time**

 Select the data Source. You can select multiple journeys in a specified time period or specify a single journey. The report presented below will be the journey report in the data source. In other words, the report can be a single trip report or a cumulative report of multiple trips.

![](../../.gitbook/assets/image%20%28521%29.png)

The report includes: 

* **Total of participants** 

Count the number of participants in the journeys of the data source. The contact’s participation in the journey is recorded as a touch. A contact can participate in the journey again after completing the journey. At this time, the number of touch will be counted up without duplicate removal. 

* **Milestones hits**

 Any step in the journey can be set as a milestone, which is used to count the number of contacts who have reached key nodes in the journey. The behavior of the contact reaching the milestone of the journey is recorded as a milestone hit. A journey may contain multiple milestones. The number of milestone hits will be counted up without duplicate removal. 

**Milestones usually refer to the core steps or core nodes in a journey. You can freely mark related controls as milestones.**

![](../../.gitbook/assets/image%20%28510%29.png)

* **24-hour performance**

The time period distribution of the recipient response events of the different channels. You can view which time period the contacts are generally more active and then optimize the sending time of the contents.

![](../../.gitbook/assets/image%20%28499%29.png)

* **Email performance** 

Display the number of recipients in each step in the email marketing process. 

* **WeChat performance** 

Display the number of recipients in each step in the WeChat marketing process. 

* **SMS click conversion**

Display the number of recipients in each step of the SMS marketing process \(including overseas\). 

* **MMS performance** 

Display the number of recipients in each step in the MMS marketing process.

![](../../.gitbook/assets/image%20%28494%29.png)

_NOTE_ 

_The above data are all be counted in the next day._

### View the EDM Delivery Report

**Step 1**Choose Data center &gt; Campaign report from the main menu. Select the Messages list tab on the top navigation bar to enter the sending list page.

![](../../.gitbook/assets/image%20%28498%29.png)

**Step 2** Select the data Source. You can select multiple journeys in a specified time period or specify a single journey. The sending status of each channel will be displayed in the list below.

**Step 3** Click Task list of the Email channel to view the email report, and similarly, click Task list of other channels to view the corresponding report.

![](../../.gitbook/assets/image%20%28501%29.png)

**Step 4**  You can find the Task name of the report you want to view in the task list page. View/ download the report.

![](../../.gitbook/assets/image%20%28539%29.png)

**Step 5** Enter the email report details page. Click to select two tasks and compare reports.

![](../../.gitbook/assets/image%20%28504%29.png)

The following is the content of the mail report: 

* **Summary**

![](../../.gitbook/assets/image%20%28500%29.png)

![](../../.gitbook/assets/image%20%28531%29.png)

**What is the difference between open and render?** 

The basis for judging whether to open the email is whether to load the hidden tracking pixel in the email. Some mail clients do not load images by default \(such as Outlook\). Therefore, by default the opened mail without clicking on any hyperlink in the email will not be counted as open or render. If the pixel image is not loaded but the email hyperlink is clicked, it will be counted in the open and click statistics, but no Open Email event will be generated at this time. After the pixel image is loaded, it will be counted as open and render. 

* **Email performance** 

Display the statistics of the number of contacts of sent, delivered, opened, and clicked after the email was sent. You can view the effect of the sent email through the statistical funnel.

![](../../.gitbook/assets/image%20%28529%29.png)

* **Email service providers radio** 

Service provider statistics of recipient mailboxes. You can check the number and proportion of recipients of each service provider.

![](../../.gitbook/assets/image%20%28535%29.png)

* **Open device ratio** 

Statistics of the recipient’s device to open the mailbox, such as PC, mobile or others.

![](../../.gitbook/assets/image%20%28506%29.png)

* **EDM opening/ clicking situation in different countries**

 Count the number of opens and clicks in different countries according to the national latitude.

![](../../.gitbook/assets/image%20%28520%29.png)

* **Custom a report**

Dmartech support custom reports in order to meet the different report needs of users. Click Create a new report at the bottom of the page to create. Set the Index and User properties to analysis the report.

![](../../.gitbook/assets/image%20%28513%29.png)

_NOTE_ 

_Only the single time journey and the cycle journey have task details of the report. There is no report for the real-time journey._

### **Export the Report** 

Choose Data center &gt; Campaign report from the main menu. Select the Export Data tab on the top navigation bar to enter the Export raw data page. This module is used to export various sending reports of emails, SMS and MMS. 

### **Export the Email Report** 

* Marketing raw data 

Export the original sending data of the specified mail task according to the mail sending indicators \(All type, sent, open, click, soft bounces, hard bounces, unsubscribe\). For example, export the voucher\_code, Organization\_PACD and Name\_PACD of the contacts who opened the mail named 2008\_IN\_Webinar\_IdeaHub\_en.

![](../../.gitbook/assets/image%20%28512%29.png)

* Types: All type, sent, open, click, soft bounces, hard bounces, unsubscribe. 
* Automations: Select a journey within a period of time or directly specify a journey, up to 4 journeys can be selected. 
* Select Email: Select the mail task in the journey. 
* Special indicator: Select the contact attributes to be exported. 
* Send time: Set the sending time of the report. 
* Format type: Set the file type of the report. Excel and CSV are supported. 
* Email subject: The default is Email raw data export notification. 
* Email address: Set the email address for receiving the export notification. Click the download link in the email to download the report.

_NOTE_ 

* _Multiple opens and clicks will be displayed repeatedly in the raw data._ 
* _A zip file will be downloaded when multiple journeys are selected._

**Email send detail**

![](../../.gitbook/assets/image%20%28502%29.png)

The header of the downloaded file:

![](../../.gitbook/assets/image%20%28497%29.png)

* Mail comparison data

![](../../.gitbook/assets/image%20%28516%29.png)


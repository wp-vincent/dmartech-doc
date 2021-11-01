# View the Journey Report

You can view and download reports related to marketing journeys and channels in Campaign report module. Choose Data center > Campaign report from the main menu to enter the Journey report review page, which includes three tab pages: Automation overview, Messages list, Export Data.

**View the Report of All Journeys or Specified Journeys within a Certain Period of Time**

&#x20;Select the data Source. You can select multiple journeys in a specified time period or specify a single journey. The report presented below will be the journey report in the data source. In other words, the report can be a single trip report or a cumulative report of multiple trips.

![](<../.gitbook/assets/image (535).png>)

The report includes:&#x20;

* **Total of participants**&#x20;

Count the number of participants in the journeys of the data source. The contact’s participation in the journey is recorded as a touch. A contact can participate in the journey again after completing the journey. At this time, the number of touch will be counted up without duplicate removal.&#x20;

* **Milestones hits**

&#x20;Any step in the journey can be set as a milestone, which is used to count the number of contacts who have reached key nodes in the journey. The behavior of the contact reaching the milestone of the journey is recorded as a milestone hit. A journey may contain multiple milestones. The number of milestone hits will be counted up without duplicate removal.&#x20;

**Milestones usually refer to the core steps or core nodes in a journey. You can freely mark related controls as milestones.**

![](<../.gitbook/assets/image (519).png>)

* **24-hour performance**

The time period distribution of the recipient response events of the different channels. You can view which time period the contacts are generally more active and then optimize the sending time of the contents.

![](<../.gitbook/assets/image (506).png>)

* **Email performance **

Display the number of recipients in each step in the email marketing process.&#x20;

* **WeChat performance **

Display the number of recipients in each step in the WeChat marketing process.&#x20;

* **SMS click conversion**

Display the number of recipients in each step of the SMS marketing process (including overseas).&#x20;

* **MMS performance**&#x20;

Display the number of recipients in each step in the MMS marketing process.

![](<../.gitbook/assets/image (497).png>)

_NOTE _

_The above data are all be counted in the next day._

### View the EDM Delivery Report

**Step 1**Choose Data center > Campaign report from the main menu. Select the Messages list tab on the top navigation bar to enter the sending list page.

![](<../.gitbook/assets/image (503).png>)

**Step 2 **Select the data Source. You can select multiple journeys in a specified time period or specify a single journey. The sending status of each channel will be displayed in the list below.

**Step 3** Click Task list of the Email channel to view the email report, and similarly, click Task list of other channels to view the corresponding report.

![](<../.gitbook/assets/image (508).png>)

**Step 4**  You can find the Task name of the report you want to view in the task list page. View/ download the report.

![](<../.gitbook/assets/image (564).png>)

**Step 5** Enter the email report details page. Click to select two tasks and compare reports.

![](<../.gitbook/assets/image (512).png>)

The following is the content of the mail report:&#x20;

* **Summary**

![](<../.gitbook/assets/image (507).png>)

![](<../.gitbook/assets/image (551).png>)

**What is the difference between open and render? **

The basis for judging whether to open the email is whether to load the hidden tracking pixel in the email. Some mail clients do not load images by default (such as Outlook). Therefore, by default the opened mail without clicking on any hyperlink in the email will not be counted as open or render. If the pixel image is not loaded but the email hyperlink is clicked, it will be counted in the open and click statistics, but no Open Email event will be generated at this time. After the pixel image is loaded, it will be counted as open and render.&#x20;

* **Email performance**&#x20;

Display the statistics of the number of contacts of sent, delivered, opened, and clicked after the email was sent. You can view the effect of the sent email through the statistical funnel.

![](<../.gitbook/assets/image (545).png>)

* **Email service providers radio **

Service provider statistics of recipient mailboxes. You can check the number and proportion of recipients of each service provider.

![](<../.gitbook/assets/image (558).png>)

* **Open device ratio **

Statistics of the recipient’s device to open the mailbox, such as PC, mobile or others.

![](<../.gitbook/assets/image (514).png>)

* **EDM opening/ clicking situation in different countries**

&#x20;Count the number of opens and clicks in different countries according to the national latitude.

![](<../.gitbook/assets/image (534).png>)

* **Custom a report**

Dmartech support custom reports in order to meet the different report needs of users. Click Create a new report at the bottom of the page to create. Set the Index and User properties to analysis the report.

![](<../.gitbook/assets/image (524).png>)

_NOTE _

_Only the single time journey and the cycle journey have task details of the report. There is no report for the real-time journey._

### **Export the Report **

Choose Data center > Campaign report from the main menu. Select the Export Data tab on the top navigation bar to enter the Export raw data page. This module is used to export various sending reports of emails, SMS and MMS.&#x20;

### **Export the Email Report**&#x20;

* Marketing raw data&#x20;

Export the original sending data of the specified mail task according to the mail sending indicators (All type, sent, open, click, soft bounces, hard bounces, unsubscribe).&#x20;



* Types: All type, sent, open, click, soft bounces, hard bounces, unsubscribe.&#x20;
* Automations: Select a journey within a period of time or directly specify a journey, up to 4 journeys can be selected.&#x20;
* Select Email: Select the mail task in the journey.&#x20;
* Special indicator: Select the contact attributes to be exported.&#x20;
* Send time: Set the sending time of the report.&#x20;
* Format type: Set the file type of the report. Excel and CSV are supported.&#x20;
* Email subject: The default is Email raw data export notification.&#x20;
* Email address: Set the email address for receiving the export notification. Click the download link in the email to download the report.

_NOTE _

* _Multiple opens and clicks will be displayed repeatedly in the raw data. _
* _A zip file will be downloaded when multiple journeys are selected._

**Email send detail**

![](<../.gitbook/assets/image (642).png>)

The header of the downloaded file:

![](<../.gitbook/assets/image (502).png>)

* **Mail comparison data**

![](<../.gitbook/assets/image (641).png>)

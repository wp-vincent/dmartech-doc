# Marketing Automation

Marketing automation is the core of automated marketing. By disassembling the marketing plan into marketing paths in the marketing journey can automatically judge user behavior, and then trigger different subsequent marketing content to contacts to achieve personalized marketing. 

Dmartech marketing journeys include three categories: single time journey, real-time journey, and cycle journey.

* **Single time journey**: The main use scenario of a single time journey is generally a one-time marketing campaign, which only provides multi-channel push for the established target audience. 
* **Real-time journey**: The particularity of the real-time journey is its filter criteria of starting. Only the contacts in the specified segment that trigger the specified filter criteria can enter the journey. If the specified filter criteria are not triggered, even the contacts in the segment will not enter the journey. The progress of each contact who enters the journey is also different during the journey since the trigger time of each person is different. That is, the real-time journey is triggered by user behavior and it is an automatic process driven in real time. 
* **Cycle journey**: A cycle journey is the periodic execution of a single journey. The repetitive cycle can be daily, weekly, or monthly. The common marketing scenarios of cycle journeys are membership day marketing and regular newsletter sending.

To use the marketing journey editor, the following conditions are generally required: 

* Windows 7 or higher operating system with Chrome/QQ browser and higher version IE browser 
* Mac OS 10.13.1 or higher with Chrome and Safari browsers

## Create  a journey

### create a single time journey

**Step 1** Choose **Marketing &gt; Automation** from the main menu to view journeys list page. Journeys can be managed in groups. There is a built-in group named Default group in Dmartech. Click "+" next to All grouping to create a new group by yourself: enter Group Name, select the superior group \(All grouping by default\). You can create up to 4 levels of groups under All grouping. The new journey will be created in Default group if no group is added. 

Generally, it is recommended to set groups according to marketing scene or creator or department since it is easy to find and manage journeys.

![](../.gitbook/assets/image%20%28576%29.png)

**Step 2**Click"create" to enter the Create New Automation explorer. Then choose Simple Flow tab to start a new single journey by setting following parameters: 

* **Select time zone**: Dmartech uses Beijing time\(UTC/GMT+08:00\) for domestic users by default. You can change the default time zone by choosing Account name &gt; General when necessary. 
* **Language**: Choose one of the three items: No restriction, Chinese or Others. 
* **Name**: Set the name of the journey. 
* **Folder**: To set which group will the journey belongs to, you can select an existing group by selecting Add to Folder, or you can directly create a new group by selecting Add to New Folder.

![](../.gitbook/assets/image%20%28493%29.png)

**Step 3** Click "Confirm" to enter the drag-and-drop drawing page. 

Journey drawing includes three steps: drag and drop the control — connection — set the control. That is, drag the control on the left navigation tree to the canvas on the right area one by one and place them in order, then connect the controls according to the process. First, you need to drag a Recipients control by selecting Segmentation or Account. 

* Click **Segmentation** to view the names of all created segment. Select a segment as the audience for this journey. 
* Click **Account** to view the WeChat official account bound to the current account. Select it to use all followers as the audience for this journey.

![](../.gitbook/assets/image%20%28569%29.png)

**Step 4** Drag and drop the rest of the controls \(Messages or Flow Actions\) one by one according to the marketing journey plan. For example, design according to the following process:

![](../.gitbook/assets/image%20%28513%29.png)

The restoration design during the journey is as follows:

![](../.gitbook/assets/image%20%28557%29.png)

**Step 5** Click the control and then to set details of the control. The setting of the Condition spilt control is as figure shows below:

![](../.gitbook/assets/image%20%28516%29.png)

**Step 6** Click “Start“ to confirm the settings of the journey and preview whether the contents in the journey are correct. Please make sure that the balance of the sending channel is sufficient. Then click “Start now“ after checking the confirmation to start the journey. 

There will be a prompt if the settings are wrong. Just modify the controls settings or paths according to the prompt. Generally speaking, it is necessary to pay attention to the self-consistent time such as sending time and judgment time.

![](../.gitbook/assets/image%20%28499%29.png)

* Description of A/B Test split Control Only a single time journey supports A/B testing. You can compare the different effects of multiple mails by A/B test. Select an audience and drag the A/B Test split control to the canvas.

![](../.gitbook/assets/image%20%28567%29.png)

Click to set details of the A/B Test split control. The main setting parameters are explained as follows: 1\)Element Title: A/B Test. 

2\)The test of time: Set the time to send the test mail. 

3\)Send Email: Add up to 4 test emails. You can set the subject of multiple mails uniformly after checking Unified subject and common \(AD\) Email Subject identifier. In case the checkboxes are unchecked, you can set the subject of each email separately and insert the personalized field in the subject. 

4\)From address: Set the sending address. 

5\)From name: Set the sender name by selecting or editing. 

6\)Test ratio: Set the ratio of the number of contacts to send. The ratio is up to 50%. Each mail batch equally divides the total ratio. 

7\)Evaluation index: Choose which index to use to evaluate the effect of the email. 

* The number of unique opens \(Real-time statistics\) 
* The number of unique clicks \(Real-time statistics\) 
* The number of unique clicks of the specified link \(The data for the day will be counted at 12:00 noon in the next day\) 

8\)Evaluation time: Set a time to evaluate the winning email, and immediately send the winning email to the remaining contacts.

![](../.gitbook/assets/image%20%28546%29.png)

### Create a real-time journey

**Step 1**Choose **Marketing &gt; Automation** from the main menu. Click "Create" to enter the Create New Automation explorer. Then choose Real-time Trigger tab to start a new real-time journey by setting following parameters: 

* Select time zone: Dmartech uses Beijing time\(UTC/GMT+08:00\) for domestic users by default. You can change the default time zone by choosing Account name &gt; General when necessary. 
* Name: Set the name of the journey. 
* Folder: To set which group will the journey belongs to, you can select an existing group by selecting Add to Folder, or you can directly create a new group by selecting Add to New Folder. 
* Groups: Select a segment in drop-down list or No Restriction here. Only the contacts in the segment that meet the trigger conditions can enter the journey. 
* Trigger 

1. Contact Activity indicates that the contacts in the specified group will enter the journey if they have completed the specified behavior once the journey starts. 
2. Contact Updates indicates that the contacts in the specified group will enter the journey if their labels or user attributes in Dmartech have a specified change once the journey starts. 

* If Contacts can trigger this automation more than once is checked, then contacts who have already completed this journey can enter the journey more than once. If unchecked, then the same contact can only enter the journey just for once.

![](../.gitbook/assets/image%20%28489%29.png)

**Step 2** Click "Confirm" to enter the drag-and-drop drawing page. Drag and drop the controls to canvas on the right area one by one according to the marketing journey plan. For example, design according to the following process:

![](../.gitbook/assets/image%20%28566%29.png)

![](../.gitbook/assets/image%20%28570%29.png)

**Step 3** Click each control to set the specific information of each control. For example, you need to set Schedule, Email subject and other parameters for each Messages control. It should be noted that the sending time of each content needs to be self-consistent. The event judgment time should also be considered if there has Event condition controls. You need to set the event conditions to be judged in the Event condition control, see below for details.

![](../.gitbook/assets/image%20%28530%29.png)

![](../.gitbook/assets/image%20%28496%29.png)

![](../.gitbook/assets/image%20%28488%29.png)

**Step4** Click "Start" after completing the editing. It is recommended that test whether the journey can be sent out correctly by selecting Save and Test and setting a test group \(usually internal contacts\), which can avoid causing harassment or inaccessibility to contacts due to issues during the journey execution.

![](../.gitbook/assets/image%20%28538%29.png)

**Step 5** Start the journey officially.

![](../.gitbook/assets/image%20%28543%29.png)

_NOTE_

 _Real-time journeys can be copied via clicking in the Options column of the journeys list page. A new journey named journey name\_copy will be generated after copying._

### Create a cycle journey

**Step 1** Choose Marketing &gt; Automation from the main menu. Click "Create" to enter the Create New Automation explorer. Then choose Recurring Flow tab to start a new cycle journey by setting following parameters: 

* Select time zone: Dmartech uses Beijing time \(UTC/GMT+08:00\) for domestic users by default. You can change the default time zone by choosing Account name &gt; General when necessary. 
* Language: Choose one of the three items: No restriction, Chinese or Others. 
* Name: Set the name of the journey. 
* Folder: To set which group will the journey belongs to, you can select an existing group by selecting Add to Folder, or you can directly create a new group by selecting Add to New Folder. 
* Repetition period: You can choose to execute the journey by day, week or month, then set the repetition period, finally set the ending method by frequency or specific time.

![](../.gitbook/assets/image%20%28562%29.png)

Step2 Click "Confirm" to enter the journey drawing page. The drawing steps are exactly same as the single time journey. Please refer to Create a Single Time Journey.

### Journey Approval

All journeys are subject to the approval process if Automation approval workflow is enabled in Enterprise Settings &gt; System Settings. 

* Applicant's perspective After creating the journey, click "Apply for apporval" at the top right corner to select an approver to submit for approval. The Status of the journey will turn to Pending after submission, which can be withdraw before being approved. 

Dmartech no longer provides a direct opening portal, opening must be approved; _Note: trips handed over to the main account for approval also need to be approved and cannot be opened directly._

You can check the approval status in the journey group named My Requests.

The Start or Continue buttons will no longer be displayed for trips that are pending approval, or have a record of approval passed or approval denied.

![](../.gitbook/assets/image%20%28531%29.png)

* Approver's perspective 

An Approver is a user who has been given rights to approve or deny journey requests from their department or team.

 You can view the pending approved journey in the journey group named My Approvals.

 Click “Examination“ to process the approval in the Prepare for launch explorer. There are three optional actions for approval: Approve, Send back \(you can input the reason for denial\), Add an approver \(choose another approver\).

~~_The journey will start directly and its status will be updated to Running once the request has been approved._~~


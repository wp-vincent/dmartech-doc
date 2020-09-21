# Data Analysis

## Dashboard

Dashboard can help you create your own dashboard. A dashboard can include multiple reports. Each account can be set to focus on several data reports in one dashboard. 

Click Data analysis &gt; Dashboard enter dashboard to manage and create pages.

 Users can add components as many as they want. In order to manage dashboards properly, it is suggested that you group your dashboards to avoid missing key data.

![](.gitbook/assets/image%20%28504%29.png)

Each dashboard includes: dashboard name, the number of reports in the dashboard, the creator, the number of views and create time. Click dashboard name can enter dashboard and view detailed reports. 

### Create dashboard 

**Step 1** Click add dashboard on the upper left corner. After entering the name, you can create a dashboard. The latest dashboard will be shown on the top. 

**Step 2** Click dashboard name to enter the dashboard page. You have to add report group firstly. After typing in the new group name, click confirm. Then you have your first report group. 

**Step 3** Click + on the top right corner of the page to create report components. You can choose components from bookmarks \(which is bookmarks generated through attribute analysis, event analysis and visualization report\) or you can create a new component. 

## Event analysis 

Event analysis is used to generate analysis reports according to the setting related analyzed conditions for arbitrary contact events. Event analysis is able to analyze events from meta data. It includes two parts which are condition setting and data analysis. 

**Step 1**Click Data analysis &gt; Event analysis enter event analysis page. There are three setting conditions, \[index\], \[grouping\] and \[filter condition\]. \[Index\] indicates the total times the specific event happens, number of triggered users or average number of times. When hovering your mouse over index icon to view the adding index for different events button. Then you are able to add conditions. 

\[Grouping\] is based on the user attribute or event attribute groups. \[Filter condition\] is used for setting user attributes related conditions with the conditions set in index. Click Data analysis &gt; Event analysis enter event analysis page. There are three setting conditions, \[index\], \[grouping\] and \[filter condition\]. 

**Step 2** When you finish step 1, click ‘run’ on the right upper corner. A chart will be generated. You can choose chart type. 

**Step 3** Click Save As Bookmark button on the top right corner to save the current chart as a bookmark. Choosing bookmark can view the chart when you creating dashboard. In addition, downloading raw data in csv format is also supported.

![](.gitbook/assets/image%20%28533%29.png)

### The examples of event analysis 

Q: What should I do if I want to know the number of events for sending? 

A: If you want to know the total sending number, you should set: Send Email of Arbitrary events demonstrated as total number of sending. 

Q: What should I do if I want to know the number of events for opening? 

A: If you want to know the total opening number, you should set: Open Email of Arbitrary events demonstrate as total number of opening. 

Q: What should I do if I want to know the number of events for soft bounce? 

A: If you want to know the total opening number, you should set: Email Softbounce of Arbitrary events demonstrate as spam complain. 

Q: What should I do if I want to know the number of events for email clicking? 

A: If you want to know the total clicking number, you should set: Click Email of Arbitrary events demonstrate as email clicking.

![](.gitbook/assets/image%20%28498%29.png)

When you click run, you can set the x-axis and y-axis by yourself. Then you can see the chart below.

![](.gitbook/assets/image%20%28520%29.png)

The table under the chart is the event occurrence table.

![](.gitbook/assets/image%20%28556%29.png)

### Contacts analysis 

Contact analysis is to generate analyzed figures such as curve chart, histogram, donut chart and pie chart by setting contact attributes and attribute conditions.

 Contact analysis is based on user attributes. Similar as event analysis, contact analysis is composed of condition setting part and data analysis part. 

Click Data analysis then click contact analysis. The steps are same as event analysis. 

**Step 1** Click setting condition to unfold condition setting. There are three setting conditions: \[display\], \[grouping\] and \[filter condition\]. \[Display\] means the contact attribute we are going to analyze. It is supported to have raw data \(duplicated\) or the deduplicated number in display. 

**Step 2** Analyze the contact attributes and generate chart. You can also save them as bookmark or download the raw data in CSV format.

![](.gitbook/assets/image%20%28554%29.png)

When you run it, the chart is shown below:

![](.gitbook/assets/image%20%28536%29.png)

## Contact group 

Contact group is used to group your contacts based on contact attribute setting or event analysis. 

Step 1Click Data analysis &gt; contact group. You can create contact group by setting the filter conditions. There are two kinds of filter conditions, \[User attribute is satisfied\] and \[done\]. \[User attribute is satisfied\] means the attribute that your contact is satisfied. \[Done\] means the user events that your contacts have done before. 

For example, if you want to filter out the contacts whose contact attributes meet the requirements that they have email, mobile phone number, and WeChat values and they open the email 3 times in the past 7 days at least once, the setting conditions are as follows: 

**Step 1** Email, mobile phone number and WeChat have values. These are contact attributes. 

**Step 2** Open the email in the past 7 days at least once is an event. Open email 3 times is event attribute.

![](.gitbook/assets/image%20%28571%29.png)

### Visualized report 

Dmartech offers various visualized reports by analysing meta data and group them. The visualized report is based on the data set.

![](.gitbook/assets/image%20%28523%29.png)

You can use different dimensions under the chart type bar. You can add all fields if you want to see all of them.


# Segmentation

In the segmentation module, contacts can be filtered into segments with the same characteristics according to different filter criteria. Contacts segments are used as the audience for the automated marketing journey, which are the basis for realizing precision marketing. Segment provides the standard segment and the advanced segment and both of them are based on user attributes and behavior events. Advanced segment is used for more complicated conditions that cannot be achieved by standard segment.

## Create a segment

Choose **Contacts &gt; Segmentation** from the main menu. The **segments list** page is displayed. Segments can be managed in groups. There is a built-in group named default group in Dmartech. Click "+" next to **All grouping** to create a new group by yourself: enter Group Name, select the superior group \(All grouping by default\). You can create up to 4 levels of groups under **All grouping**. The new segment will be created in default group if no group is added. Generally, it is recommended to set groups according to marketing scene or creator or department since it is easy to find segments and manage them.

### Create a standard segment

#### Step1 **Click "create segments"at the top right corner** 

![](../.gitbook/assets/tu-pian-5%20%281%29.png)

**Step2** Enter **segment name** and select which group will belong to 

![](../.gitbook/assets/tu-pian-6%20%281%29.png)

**Step3** Step 3Set filter criteria of the segment. To set the filter criteria about contact attributes, click the drop-down box under **Contacts attribute satisfying**... and select an attribute firstly, then select a filter criterion, and then enter the value as need. Different attribute fields correspond to different filter criteria.

![](../.gitbook/assets/tu-pian-7%20%281%29.png)

**Step4** After setting a filter criterion, click "+"to add a new filter criterion and click to delete it. The relationship between the added filter criteria is and by default. Click "and" to switch to or.

![](../.gitbook/assets/tu-pian-8%20%281%29.png)

**Step5** To set the filter criteria about behavior events, click the drop-down box under **Behavioral event satisfying**... and select an event, then "Add event attributes" will appear. Click the drop-down box below to select an attribute and set a filter criterion.

![](../.gitbook/assets/tu-pian-9%20%281%29.png)

As shown in the figure below, filter criteria are: 

* The number of emails opened is greater than or equal to 3 times from 2020-08-01 to 2020-07-30. 
* The value of location is equal to China when submitting the form named test form.

![](../.gitbook/assets/tu-pian-11%20%281%29.png)

Step 6 Click **Add Condition Bunch** to tick to add a **Contact attribute condition bunch** or a **Behavioral event condition bunch**.

![](../.gitbook/assets/tu-pian-12%20%281%29.png)

_NOTE :The relationship between conditional clusters is and, and the conditions in the cluster can be and or or._

**Step7** Click "confirm" Dmartech will quickly screen out the contacts that meet the filter criteria.

### Create an advance segment 

Some complex scenarios cannot be realized by using standard segments, so that you need to create an advanced segment. 

Advanced segments use multiple standard segments as sub-segments. Each sub-segment can be set to **include** or **exclude**: **Include** indicates that the advanced group contains contacts filtered by this sub-segment. **Exclude** indicates that the advanced group does not contain the contacts filtered by this sub-segment.

**Step1**:Click **Create ADV Segments**. In the **Create ADV Segments** dialog box, **set segment name** and **folder**.

![](../.gitbook/assets/tu-pian-13%20%281%29.png)

**Step3** Set filter criteria of the sub-segment on the right side of the page. See Create a Standard Segment for more details. For example, the filter criteria of sub-segment named a\_sub are the contacts attribute satisfies **country** is _China_ and **gender** is _female_.

![](../.gitbook/assets/tu-pian-14%20%281%29.png)

![](../.gitbook/assets/tu-pian-15%20%281%29.png)

Step4 Click **Save**. The relation between the sub-segment and the segment is **include** by default. You can switch the relation to **exclude** according to actual needs.

![](../.gitbook/assets/tu-pian-16%20%281%29.png)

**Step 5** Continue to create next sub-segment by clicking “+“. You can also directly copy an existing sub-segment and then modify the filter criteria. For example, you can select one or more segments from all segments to copy. The all sub-segments belong to an advanced segment will be copied if the advanced segment is selected.

**Step 6** Click at the top right corner to start the calculation after creating all sub-segments. Dmartech will calculate the contacts that meet the filter criteria according to the set relation between sub-segments and the advanced segment.

**Step 7** The total number of each sub-segment is displayed in the navigation area on the left. The total number of the advanced segment can be viewed in the segment list after the calculation is completed. Total number of contacts = included number-excluded number




# Meta Data

User attributes, events, and event attributes can be defined in the Meta data module. User attributes refer to various aspects information of contacts, such as name, gender, age, etc. These information can be entered when uploading or creating a contact, or obtained and imported by Dmartech when the contact submitting the form. The behavior of the contacts is recorded by events, and all behaviors and actions can be viewed in the Contact dynamic info in the Contact detail page. There are some common preset events in Dmartech. The platform will capture some contacts behavior events by default. It also supports custom events for event tracking or other event records of background transmission. There is no limit to the number of created custom events.

### Customize Contact Attributes

Dmartech presets some common contact attributes and supports to customize attributes. The customizable field types include string, integer, date, and decimal. It is necessary to set correct data type when importing contacts data by files or API, otherwise it could cause data import errors.&#x20;

All contact data fields need to be defined in the User properties page first before importing to the platform, otherwise the data will not be imported to the platform (the form fields also need to be created in the Meta data).&#x20;

Step 1Choose Data center> Meta data from the main menu. Select the User properties tab on the top navigation bar. Check whether the required contact attribute is currently exist in the user properties list. If not, click to add a new user attribute. The parameters that need to be filled when adding a new user attribute record:&#x20;

* Property name: The name of the property that stored in the database, which cannot be repeated with the existed property names.&#x20;
* Field meaning: The name displayed in Dmartech, which cannot be repeated with the existed field meanings.&#x20;
* Type: Choose one of the four types: string, integer, date and decimal.&#x20;
* Length: Set the field length according to the Type.&#x20;
* Key identify: The platform will merge data record according to the primary key attributes. If Key identify is enabled, the different records with the same primary key values will be considered as the same contact. Therefore, it is necessary to set the attribute that can represent the contacts’ identity as the primary key, such as mobile, email, etc. The primary key is unique. Attributes with repeated values cannot be defined as primary keys.&#x20;

**Step 2 **Click 'Save" to complete the creation.

![](<.gitbook/assets/image (575).png>)

### Customize Events

Custom events are generally used for event tracking or event records by API transmission.&#x20;

**Step 1**It is required to add the attributes of the event first in order to customize an event. Choose Data center> Meta data from the main menu. Select the Event properties tab on the top navigation bar. Click "Add" to create the attributes of the newly defined event by setting below parameters:&#x20;

* Property name: The english name of the property that stored in the database.&#x20;
* Field meaning: The Chinese name displayed in Dmartech.&#x20;
* Type: Choose one of the four types: string, integer, date and decimal.&#x20;
* Length: Different attributes types have different lengths.

![](<.gitbook/assets/image (542).png>)

**Step  2**  the event after creating the event properties. Select the Event management tab on the top navigation bar. Click "Add" to create an custom event by setting below parameters:&#x20;

* Event name: The name of the event that stored in the database.&#x20;
* Display name: The Chinese name displayed in Dmartech.&#x20;
* Preset property: Select the event attributes used by the event, which is used to describe the event (The event attributes has created in Step 1).

**Step 3** The created event will be stored in the default group, or you can select Event group tab to create a new group by setting below parameters:&#x20;

* Group name: Set a group name of the event.&#x20;
* Display name: Set the displayed group name.&#x20;
* Defined event: Check the custom event just created.

![](<.gitbook/assets/image (529).png>)

### Example

The group named email includes Open Email and Click Email events. The attributes of the Open Email event include journey\_template\_id, task\_instantiation\_id, event\_date, dmd\_mailing\_name, create\_date\_email, email and etc.&#x20;

The default preset events do not need to be edited. The above events will be automatically recorded when the contact has related behaviors. You can view the event record by clicking Contact dynamic in the Contact detail page.

![](<.gitbook/assets/image (537).png>)

### Scoring Management

Coming soon.......




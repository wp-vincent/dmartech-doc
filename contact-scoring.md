---
description: >-
  New "Contact Scoring" module is added to the contact management, and the new
  scoring function is online.
---

# Contact Scoring

With the new contact scoring, the original shared factors, shared models, and scoring levels are integrated and merged into a single independent scoring model in which you create your own exclusive factors; you can score all contacts as well as only new contacts; and the historical scoring results on the contacts will always be visible if the model is not deleted.

Click Contact Management and select Contact Scoring to go to the main page.

![](<.gitbook/assets/image (649).png>)

Main Page&#x20;

&#x20;\[Activated/Upper limit] shows the number of models enabled and the number of models in the limit of the account. \[Factor Templates Library] can convert the models already created into templates for saving.

![](<.gitbook/assets/image (640).png>)

【Model List】Provides model name, status (divided into Enable, Disable, Draft and All, which can only be selected singly), scoring progress (the exact length is determined by the number of contacts and channels), updater account, update time and operation bar.&#x20;

The action bar provides enable/disable, edit, report, copy and delete operations.&#x20;

* Enable/disable: draft or disable state provides enable, enable state provides disable.
* &#x20;Edit: click Edit to enter the scoring model editing page.&#x20;
* Report: model reports in non-draft state can be viewed.&#x20;
* Copy: a new model can be generated after copying.&#x20;
* Delete: models can be deleted from the deactivated and draft states.&#x20;

New Scoring Model Click the "Create Scoring Model" button at the top right corner of the page to start creating a model.

![](<.gitbook/assets/image (647).png>)

_**Note: New contacts are filtered based on the contact creation time field**_

\[Editorial scoring model].

![](<.gitbook/assets/image (648).png>)

New creation is completed or click Edit button to enter the scoring model editing page The top display shows the model's full score, the number of grades and a prompt for the scoring time The number of rating levels can be edited

![](<.gitbook/assets/image (644).png>)

Four levels are provided by default, the first and last level cannot be deleted, and up to 20 levels can be set; the lowest score of the first level can be set to -9999, and the highest score of the last level can be set to 9999.

\[List of scoring factors].

![](<.gitbook/assets/image (646).png>)

The list of scoring factors includes factor name, field or event, number of rules, scoring range and action bar, with a search box and a new scoring factor button in the upper right corner. New rating factor can be created blank or selected from the template library. You can select attribute factor or event factor and the corresponding field.

![](<.gitbook/assets/image (639).png>)

Fields are aligned with the corresponding fields of the system metadata

![](<.gitbook/assets/image (637).png>)

Edit the scoring factor, take the event factor first open email as an example, click the edit button to bring up the edit window

![](<.gitbook/assets/image (642) (1).png>)

Support to select the conditions of scoring rules, set the scoring time, select the open mailing list, as well as you can see the estimated number of people and the scoring criteria and upper limit, click OK to finish editing. The scoring factor can also be dumped as a template.&#x20;

\[Scoring Report]. Click the report button in the operation column of the scoring list to enter the scoring report page.

![](<.gitbook/assets/image (645).png>)

By default, the graphs show the trend of the number of people in each rank for the last 1 month, click on the legend to show or hide the corresponding rank curve according to your needs

If the model is not running on that day, the number of people in each rating is 0 in the graph Below the graph, the statistics after the last rating was completed are displayed, i.e. the latest rating results

![](<.gitbook/assets/image (656).png>)

Includes the total number of ratings and the most recent rating time, with a breakdown of the latest rated results and the number of people shown below. Includes rating levels, number of people, percentages and action columns.&#x20;

If a rating has never been made, the total number of people is shown as 0 and the list is also shown as empty.&#x20;

The action bar allows you to create a new subgroup directly from the contacts under that rating.

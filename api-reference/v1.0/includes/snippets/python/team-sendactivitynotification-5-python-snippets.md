---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/v1.0/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7');


requestBody.setTopic($topic);
requestBody.setActivityType('pendingFinanceApprovalRequests');

previewText = ItemBody();
previewText.setContent('Internal spending team has a pending finance approval requests');


requestBody.setPreviewText($previewText);
recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.teamMembersNotificationRecipient');

additionalData = [
'teamId' => 'e8bece96-d393-4b9b-b8da-69cedef1a7e7', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('pendingRequestCount');

templateParametersKeyValuePair1.setValue('5');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




graphServiceClient.teamsById('team-id').sendActivityNotification().post(requestBody);


```
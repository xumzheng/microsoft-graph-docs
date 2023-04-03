---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/v1.0/teams/{teamId}');


requestBody.setTopic($topic);
requestBody.setActivityType('pendingFinanceApprovalRequests');

previewText = ItemBody();
previewText.setContent('Internal spending team has a pending finance approval requests');


requestBody.setPreviewText($previewText);
recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('pendingRequestCount');

templateParametersKeyValuePair1.setValue('5');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




await client.teamsById('team-id').sendActivityNotification().post(requestBody);


```
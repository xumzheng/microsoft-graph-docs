---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}');


requestBody.setTopic($topic);
requestBody.setActivityType('reservationUpdated');

previewText = ItemBody();
previewText.setContent('You have moved up the queue');


requestBody.setPreviewText($previewText);
recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('reservationId');

templateParametersKeyValuePair1.setValue('TREEE433');


templateParametersArray []= templateParametersKeyValuePair1;
templateParametersKeyValuePair2 = KeyValuePair();
templateParametersKeyValuePair2.setName('currentSlot');

templateParametersKeyValuePair2.setValue('23');


templateParametersArray []= templateParametersKeyValuePair2;
requestBody.setTemplateParameters(templateParametersArray);




awaitclient.teamsById('team-id').sendActivityNotification().post(requestBody);


```
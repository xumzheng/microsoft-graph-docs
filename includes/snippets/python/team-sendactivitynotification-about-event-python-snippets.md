---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('text'));

topic.setValue('Weekly Virtual Social');

topic.setWebUrl('Teams webUrl');


requestBody.setTopic($topic);
previewText = ItemBody();
previewText.setContent('It will be fun!');


requestBody.setPreviewText($previewText);
requestBody.setActivityType('eventCreated');

recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.teamMembersNotificationRecipient');

additionalData = [
'teamId' => '7155e3c8-175e-4311-97ef-572edc3aa3db', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);


graphServiceClient.teamsById('team-id').sendActivityNotification().post(requestBody);


```
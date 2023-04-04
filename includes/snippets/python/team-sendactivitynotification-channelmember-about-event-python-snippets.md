---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('text'));

topic.setValue('Weekly Virtual Social');

topic.setWebUrl('Teams webUrl');


request_body.setTopic($topic);
previewText = ItemBody();
previewText.setContent('It will be fun!');


request_body.setPreviewText($previewText);
request_body.setActivityType('eventCreated');

recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.channelMembersNotificationRecipient');

additionalData = [
'teamId' => '7155e3c8-175e-4311-97ef-572edc3aa3db', 
'channelId' => '19:0ea5de04de4743bcb4cd20cb99235d99@thread.tacv2', 
];
recipient.setAdditionalData(additionalData);



request_body.setRecipient($recipient);


await client.teamsById('team-id').sendActivityNotification().post(request_body);


```
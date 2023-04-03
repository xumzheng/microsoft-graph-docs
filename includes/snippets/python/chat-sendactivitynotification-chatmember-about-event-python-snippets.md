---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

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
recipient.set@odatatype('microsoft.graph.chatMembersNotificationRecipient');

additionalData = [
'chatId' => '19:d65713bc498c4a428c71ef9353e6ce20@thread.v2', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);


await client.chatsById('chat-id').sendActivityNotification().post(requestBody);


```
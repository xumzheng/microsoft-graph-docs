---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2');


requestBody.setTopic($topic);
requestBody.setActivityType('taskCreated');

previewText = ItemBody();
previewText.setContent('New Task Created');


requestBody.setPreviewText($previewText);
recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.chatMembersNotificationRecipient');

additionalData = [
'chatId' => '19:1c3af46e9e0f4a5293343c8813c47619@thread.v2', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('taskId');

templateParametersKeyValuePair1.setValue('Task 12322');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




await client.chatsById('chat-id').sendActivityNotification().post(requestBody);


```
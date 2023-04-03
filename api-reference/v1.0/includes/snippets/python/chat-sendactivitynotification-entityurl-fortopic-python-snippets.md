---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}');


requestBody.setTopic($topic);
requestBody.setActivityType('approvalRequired');

previewText = ItemBody();
previewText.setContent('Deployment requires your approval');


requestBody.setPreviewText($previewText);
recipient = TeamworkNotificationRecipient();
recipient.set@odatatype('microsoft.graph.aadUserNotificationRecipient');

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.setAdditionalData(additionalData);



requestBody.setRecipient($recipient);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('approvalTaskId');

templateParametersKeyValuePair1.setValue('2020AAGGTAPP');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




graphServiceClient.chatsById('chat-id').sendActivityNotification().post(requestBody);


```
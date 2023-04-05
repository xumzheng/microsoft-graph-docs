---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/v1.0/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2')


request_body.setTopic($topic)
request_body.setActivityType('taskCreated')

previewText = ItemBody()
previewText.setContent('New Task Created')


request_body.setPreviewText($previewText)
recipient = TeamworkNotificationRecipient()
recipient.set@odatatype('microsoft.graph.chatMembersNotificationRecipient')

additionalData = [
'chatId' => '19:1c3af46e9e0f4a5293343c8813c47619@thread.v2', 
];
recipient.setAdditionalData(additionalData)



request_body.setRecipient($recipient)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('taskId')

templateParametersKeyValuePair1.setValue('Task 12322')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)




await client.chatsby_id('chat-id').sendActivityNotification.post(request_body)


```
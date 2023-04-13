---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2'


request_body.topic = topic
request_body.activityType = 'taskCreated'

preview_text = ItemBody()
previewText.content = 'New Task Created'


request_body.preview_text = previewText
recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.chatMembersNotificationRecipient'

additionalData = [
'chatId' => '19:1c3af46e9e0f4a5293343c8813c47619@thread.v2', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient
template_parameters_key_value_pair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'taskId'

templateParametersKeyValuePair1.value = 'Task 12322'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.chats_by_id('chat-id').sendActivityNotification.post(request_body = request_body)


```
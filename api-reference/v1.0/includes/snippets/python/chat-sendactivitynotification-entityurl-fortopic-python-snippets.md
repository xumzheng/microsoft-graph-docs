---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}'


request_body.topic = topic
request_body.activityType = 'approvalRequired'

previewText = ItemBody()
previewText.content = 'Deployment requires your approval'


request_body.previewText = previewText
recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.aadUserNotificationRecipient'

additionalData = [
'userId' => '569363e2-4e49-4661-87f2-16f245c5d66a', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'approvalTaskId'

templateParametersKeyValuePair1.value = '2020AAGGTAPP'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)




request_configuration = SendActivityNotificationRequestBuilderPostRequestConfiguration(
)


await client.chats_by_id('chat-id').sendActivityNotification.post(request_body = request_body)


```
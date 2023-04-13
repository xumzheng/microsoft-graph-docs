---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('text'))

topic.value = 'Weekly Virtual Social'

topic.webUrl = 'Teams webUrl'


request_body.topic = topic
previewText = ItemBody()
previewText.content = 'It will be fun!'


request_body.previewText = previewText
request_body.activityType = 'eventCreated'

recipient = TeamworkNotificationRecipient()
recipient.@odatatype = 'microsoft.graph.chatMembersNotificationRecipient'

additionalData = [
'chatId' => '19:d65713bc498c4a428c71ef9353e6ce20@thread.v2', 
];
recipient.additionaldata(additionalData)



request_body.recipient = recipient



await client.chats_by_id('chat-id').sendActivityNotification.post(request_body = request_body)


```
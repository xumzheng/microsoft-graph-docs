---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Send_activity_notification_post_request_body()
topic = Teamwork_activity_topic()
topic.source(TeamworkActivityTopicSource.Text('teamworkactivitytopicsource.text'))

topic.value = 'Weekly Virtual Social'

topic.web_url = 'Teams webUrl'


request_body.topic = topic
preview_text = Item_body()
preview_text.content = 'It will be fun!'


request_body.preview_text = preview_text
request_body.activity_type = 'eventCreated'

recipient = Teamwork_notification_recipient()
recipient.@odata_type = 'microsoft.graph.chatMembersNotificationRecipient'

additional_data = [
'chat_id' => '19:d65713bc498c4a428c71ef9353e6ce20@thread.v2', 
];
recipient.additional_data(additional_data)



request_body.recipient = recipient



await client.chats.by_chat_id('chat-id').send_activity_notification.post(request_body = request_body)


```
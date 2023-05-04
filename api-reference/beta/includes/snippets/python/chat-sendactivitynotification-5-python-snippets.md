---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Send_activity_notification_post_request_body()
topic = Teamwork_activity_topic()
topic.source(TeamworkActivityTopicSource.EntityUrl('teamworkactivitytopicsource.entityurl'))

topic.value = 'https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2'


request_body.topic = topic
request_body.activity_type = 'taskCreated'

preview_text = Item_body()
preview_text.content = 'New Task Created'


request_body.preview_text = preview_text
recipient = Teamwork_notification_recipient()
recipient.@odata_type = 'microsoft.graph.chatMembersNotificationRecipient'

additional_data = [
'chat_id' => '19:1c3af46e9e0f4a5293343c8813c47619@thread.v2', 
];
recipient.additional_data(additional_data)



request_body.recipient = recipient
template_parameters_key_value_pair1 = Key_value_pair()
template_parameters_key_value_pair1.name = 'taskId'

template_parameters_key_value_pair1.value = 'Task 12322'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.chats.by_chat_id('chat-id').send_activity_notification.post(request_body = request_body)


```
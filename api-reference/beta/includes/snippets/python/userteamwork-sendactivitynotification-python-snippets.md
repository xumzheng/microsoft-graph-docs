---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Send_activity_notification_post_request_body()
topic = Teamwork_activity_topic()
topic.source(TeamworkActivityTopicSource.EntityUrl('teamworkactivitytopicsource.entityurl'))

topic.value = 'https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}'


request_body.topic = topic
request_body.activity_type = 'taskCreated'

preview_text = Item_body()
preview_text.content = 'New Task Created'


request_body.preview_text = preview_text
template_parameters_key_value_pair1 = Key_value_pair()
template_parameters_key_value_pair1.name = 'taskId'

template_parameters_key_value_pair1.value = 'Task 12322'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.users.by_user_id('user-id').teamwork.send_activity_notification.post(request_body = request_body)


```
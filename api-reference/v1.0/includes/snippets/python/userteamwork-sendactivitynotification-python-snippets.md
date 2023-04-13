---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.Source(TeamworkActivityTopicSource('entityurl'))

topic.value = 'https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}'


request_body.topic = topic
request_body.activityType = 'taskCreated'

preview_text = ItemBody()
previewText.content = 'New Task Created'


request_body.preview_text = previewText
template_parameters_key_value_pair1 = KeyValuePair()
templateParametersKeyValuePair1.name = 'taskId'

templateParametersKeyValuePair1.value = 'Task 12322'


templateParametersArray []= templateParametersKeyValuePair1;
request_body.templateparameters(templateParametersArray)





await client.users_by_id('user-id').teamwork.sendActivityNotification.post(request_body = request_body)


```
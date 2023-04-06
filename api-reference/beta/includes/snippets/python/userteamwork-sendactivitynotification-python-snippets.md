---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SendActivityNotificationPostRequestBody()
topic = TeamworkActivityTopic()
topic.setSource(TeamworkActivityTopicSource('entityurl'))

topic.setValue('https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}')


request_body.setTopic($topic)
request_body.setActivityType('taskCreated')

previewText = ItemBody()
previewText.setContent('New Task Created')


request_body.setPreviewText($previewText)
templateParametersKeyValuePair1 = KeyValuePair()
templateParametersKeyValuePair1.setName('taskId')

templateParametersKeyValuePair1.setValue('Task 12322')


templateParametersArray []= templateParametersKeyValuePair1;
request_body.setTemplateParameters(templateParametersArray)



request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(
request_config = SendActivityNotificationRequestBuilderPostRequestConfiguration(query_params=)


await client.users_by_id('user-id').teamwork.sendActivityNotification.post(request_body, headers=)


```
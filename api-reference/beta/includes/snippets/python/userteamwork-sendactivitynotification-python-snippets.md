---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SendActivityNotificationPostRequestBody();
topic = TeamworkActivityTopic();
topic.setSource(TeamworkActivityTopicSource('entityurl'));

topic.setValue('https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}');


requestBody.setTopic($topic);
requestBody.setActivityType('taskCreated');

previewText = ItemBody();
previewText.setContent('New Task Created');


requestBody.setPreviewText($previewText);
templateParametersKeyValuePair1 = KeyValuePair();
templateParametersKeyValuePair1.setName('taskId');

templateParametersKeyValuePair1.setValue('Task 12322');


templateParametersArray []= templateParametersKeyValuePair1;
requestBody.setTemplateParameters(templateParametersArray);




graphServiceClient.usersById('user-id').teamwork().sendActivityNotification().post(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = OutlookTask();
dueDateTime = DateTimeTimeZone();
dueDateTime.setDateTime('2016-05-06T16:00:00');

dueDateTime.setTimeZone('Eastern Standard Time');


requestBody.setDueDateTime($dueDateTime);

requestConfiguration = OutlookTaskRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'outlook.timezone="Eastern Standard Time"',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().outlook().tasksById('outlookTask-id').patch(requestBody, requestConfiguration);


```
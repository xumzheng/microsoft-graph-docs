---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = OutlookTask();
dueDateTime = DateTimeTimeZone();
dueDateTime.setDateTime('2016-05-06T16:00:00');

dueDateTime.setTimeZone('Eastern Standard Time');


requestBody.setDueDateTime($dueDateTime);

request_config = OutlookTaskRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'outlook.timezone="Eastern Standard Time"',
];

request_config.headers = headers;


result = awaitclient.me().outlook().tasksById('outlookTask-id').patch(requestBody, request_config);


```
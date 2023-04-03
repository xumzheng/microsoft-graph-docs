---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OutlookTask();
requestBody.setSubject('Shop for children\'s weekend');

startDateTime = DateTimeTimeZone();
startDateTime.setDateTime('2016-05-03T09:00:00');

startDateTime.setTimeZone('Eastern Standard Time');


requestBody.setStartDateTime($startDateTime);
dueDateTime = DateTimeTimeZone();
dueDateTime.setDateTime('2016-05-05T16:00:00');

dueDateTime.setTimeZone('Eastern Standard Time');


requestBody.setDueDateTime($dueDateTime);

request_config = TasksRequestBuilderPostRequestConfiguration();

headers = [
	'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

request_config.headers = headers;


result = await client.me().outlook().tasks().post(requestBody, request_config);


```
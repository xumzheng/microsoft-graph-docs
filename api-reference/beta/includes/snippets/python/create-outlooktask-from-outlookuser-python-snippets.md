---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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

requestConfiguration = TasksRequestBuilderPostRequestConfiguration();

headers = [
	'Prefer' => 'outlook.timezone="Pacific Standard Time"',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.me().outlook().tasks().post(requestBody, requestConfiguration);


```
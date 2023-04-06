---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OutlookTask()
request_body.setSubject('Shop for children\'s weekend')

startDateTime = DateTimeTimeZone()
startDateTime.setDateTime('2016-05-03T09:00:00')

startDateTime.setTimeZone('Eastern Standard Time')


request_body.setStartDateTime($startDateTime)
dueDateTime = DateTimeTimeZone()
dueDateTime.setDateTime('2016-05-05T16:00:00')

dueDateTime.setTimeZone('Eastern Standard Time')


request_body.setDueDateTime($dueDateTime)

request_configuration = TasksRequestBuilderPostRequestConfiguration(
request_configuration = TasksRequestBuilderPostRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.me.outlook.tasks.post(request_body, request_configuration)


```
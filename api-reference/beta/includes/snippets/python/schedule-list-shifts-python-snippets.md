---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = ShiftsRequestBuilderGetRequestConfiguration(
request_configuration = ShiftsRequestBuilderGetRequestConfiguration(query_params=query_params = ShiftsRequestBuilderGetQueryParameters()
query_params['filter'] = "sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z"

)
query_params = ShiftsRequestBuilderGetQueryParameters()
query_params['filter'] = "sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z"

)


result = await client.teams_by_id('team-id').schedule.shifts.get(request_configuration)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = TimesOffRequestBuilderGetRequestConfiguration(
request_config = TimesOffRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z"
)


result = await client.teams_by_id('team-id').schedule.timesOff.get(request_config, headers=request_config)


```
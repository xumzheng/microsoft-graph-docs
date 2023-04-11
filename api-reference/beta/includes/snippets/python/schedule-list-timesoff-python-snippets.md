---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = TimesOffRequestBuilder.TimesOffRequestBuilderGetQueryParameters(
				filter = "sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z",
)

request_configuration = TimesOffRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.teams_by_id('team-id').schedule.timesOff.get(request_configuration = request_configuration)


```
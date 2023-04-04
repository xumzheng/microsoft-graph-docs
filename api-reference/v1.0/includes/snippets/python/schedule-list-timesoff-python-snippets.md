---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = TimesOffRequestBuilderGetRequestConfiguration();

query_params = TimesOffRequestBuilderGetQueryParameters;
query_params.filter = "sharedTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and sharedTimeOff/endDateTime le 2019-03-18T00:00:00.000Z and draftTimeOff/startDateTime ge 2019-03-11T00:00:00.000Z and draftTimeOff/endDateTime le 2019-03-18T00:00:00.000Z";

request_config.queryParameters = query_params;


result = await client.teamsById('team-id').schedule().timesOff().get(request_config);


```
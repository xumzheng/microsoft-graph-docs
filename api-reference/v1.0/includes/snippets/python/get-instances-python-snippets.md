---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = InstancesRequestBuilderGetRequestConfiguration();

query_params = InstancesRequestBuilderGetQueryParameters();
query_params.startDateTime = "2019-04-08T09:00:00.0000000";
query_params.endDateTime = "2019-04-30T09:00:00.0000000";
query_params.select = ["subject","bodyPreview","seriesMasterId","type","recurrence","start","end"];

request_config.queryParameters = query_params;


result = await client.me.eventsById('event-id').instances.get(request_config);


```
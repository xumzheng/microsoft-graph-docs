---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = InstancesRequestBuilderGetRequestConfiguration(
request_configuration = InstancesRequestBuilderGetRequestConfiguration(query_params=query_params = InstancesRequestBuilderGetQueryParameters()
query_params['startDateTime'] = "2019-04-08T09:00:00.0000000"
query_params['endDateTime'] = "2019-04-30T09:00:00.0000000"
query_params['select'] = ["subject","bodyPreview","seriesMasterId","type","recurrence","start","end"]

)
query_params = InstancesRequestBuilderGetQueryParameters()
query_params['startDateTime'] = "2019-04-08T09:00:00.0000000"
query_params['endDateTime'] = "2019-04-30T09:00:00.0000000"
query_params['select'] = ["subject","bodyPreview","seriesMasterId","type","recurrence","start","end"]

)


result = await client.me.events_by_id('event-id').instances.get(request_configuration)


```
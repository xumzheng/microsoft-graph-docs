---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerBucket()
request_body.setName('Development')


request_config = PlannerBucketRequestBuilderPatchRequestConfiguration(
request_config = PlannerBucketRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.buckets_by_id('plannerBucket-id').patch(request_body, request_config, headers=request_config)


```
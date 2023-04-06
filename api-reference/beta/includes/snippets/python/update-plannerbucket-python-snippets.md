---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerBucket()
request_body.setName('Development')


request_configuration = PlannerBucketRequestBuilderPatchRequestConfiguration(
request_configuration = PlannerBucketRequestBuilderPatchRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.planner.buckets_by_id('plannerBucket-id').patch(request_body, request_configuration)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = PlannerBucketRequestBuilderDeleteRequestConfiguration()

headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
]

request_config.headers = headers


await client.planner.bucketsby_id('plannerBucket-id').delete(request_config)


```
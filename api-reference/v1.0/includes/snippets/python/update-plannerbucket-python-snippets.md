---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerBucket()
request_body.setName('Development')


request_config = PlannerBucketRequestBuilderPatchRequestConfiguration()

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
]

request_config.headers = headers


result = await client.planner.bucketsById('plannerBucket-id').patch(request_body, request_config)


```
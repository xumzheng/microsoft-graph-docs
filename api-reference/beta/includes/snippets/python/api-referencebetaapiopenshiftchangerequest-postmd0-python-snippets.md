---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShiftChangeRequest()
request_body.setSenderMessage('Can I take this shift?')

request_body.setOpenShiftId('577b75d2-a927-48c0-a5d1-dc984894e7b8')


request_config = OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration()

headers = [
	'Authorization' => 'Bearer {token}',
]

request_config.headers = headers


result = await client.teamsby_id('team-id')_schedule_openShiftChangeRequests.post(request_body, request_config)


```
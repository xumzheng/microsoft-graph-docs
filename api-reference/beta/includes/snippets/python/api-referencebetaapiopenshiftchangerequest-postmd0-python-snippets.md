---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OpenShiftChangeRequest()
request_body.senderMessage = 'Can I take this shift?'

request_body.openShiftId = '577b75d2-a927-48c0-a5d1-dc984894e7b8'



request_configuration = OpenShiftChangeRequestsRequestBuilderPostRequestConfiguration(
headers = {
					'Authorization' : "Bearer {token}",
}

)


result = await client.teams_by_id('team-id').schedule.openShiftChangeRequests.post(request_body = request_body, request_configuration = request_configuration)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = OfferShiftRequest()
request_body.senderShiftId = 'SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29'

request_body.senderMessage = 'Having a family emergency, could you take this shift for me?'

request_body.recipientUserId = 'fe278b61-21ac-4872-8b41-1962bbb98e3c'



request_configuration = OfferShiftRequestsRequestBuilder.OfferShiftRequestsRequestBuilderPostRequestConfiguration(
headers = {
		'Authorization' : "Bearer {token}",
}

)


result = await client.teams_by_id('team-id').schedule.offerShiftRequests.post(request_body = request_body, request_configuration = request_configuration)


```
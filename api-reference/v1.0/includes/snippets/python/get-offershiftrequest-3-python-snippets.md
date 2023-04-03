---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = OfferShiftRequest();
requestBody.setSenderShiftId('SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29');

requestBody.setSenderMessage('Having a family emergency, could you take this shift for me?');

requestBody.setRecipientUserId('fe278b61-21ac-4872-8b41-1962bbb98e3c');


request_config = OfferShiftRequestsRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {token}',
];

request_config.headers = headers;


result = await client.teamsById('team-id').schedule().offerShiftRequests().post(requestBody, request_config);


```
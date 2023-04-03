---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SwapShiftsChangeRequest();
requestBody.setSenderShiftId('5ad10161-6524-4c7c-9beb-4e8677ba2f6d');

requestBody.setSenderMessage('I can\'t make my shift, any chance we can swap?');

requestBody.setRecipientUserId('567c8ea5-9e32-422a-a663-8270201699cd');

requestBody.setRecipientShiftId('e73408ca-3ea5-4bbf-96a8-2e06c95f7a2c');


request_config = SwapShiftsChangeRequestsRequestBuilderPostRequestConfiguration();

headers = [
	'Authorization' => 'Bearer {token}',
];

request_config.headers = headers;


result = await client.teamsById('team-id').schedule().swapShiftsChangeRequests().post(requestBody, request_config);


```
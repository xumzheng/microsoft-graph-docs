---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new OfferShiftRequest();
$requestBody.setSenderShiftId('SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29');

$requestBody.setSenderMessage('Having a family emergency, could you take this shift for me?');

$requestBody.setRecipientUserId('fe278b61-21ac-4872-8b41-1962bbb98e3c');


$requestConfiguration = new OfferShiftRequestsRequestBuilderPostRequestConfiguration();

$headers = [
	'Authorization' => 'Bearer {token}',
];

$requestConfiguration.headers = $headers;


$requestResult = $graphServiceClient.teamsById('team-id').schedule().offerShiftRequests().post($requestBody, $requestConfiguration);


```
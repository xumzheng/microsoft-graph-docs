---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new RejectPostRequestBody();
$requestBody->setReason(new RejectReason('none'));



$graphServiceClient->communications()->callsById('call-id')->reject()->post($requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new UpdateAdDomainPasswordPostRequestBody();
$requestBody.setAdDomainPassword('AdDomainPassword value');



$graphServiceClient.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').updateAdDomainPassword().post($requestBody);


```
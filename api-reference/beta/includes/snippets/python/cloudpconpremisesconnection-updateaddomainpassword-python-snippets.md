---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = UpdateAdDomainPasswordPostRequestBody();
requestBody.setAdDomainPassword('AdDomainPassword value');



await client.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').updateAdDomainPassword().post(requestBody);


```
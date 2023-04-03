---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UpdateAdDomainPasswordPostRequestBody();
requestBody.setAdDomainPassword('AdDomainPassword value');



awaitclient.deviceManagement().virtualEndpoint().onPremisesConnectionsById('cloudPcOnPremisesConnection-id').updateAdDomainPassword().post(requestBody);


```
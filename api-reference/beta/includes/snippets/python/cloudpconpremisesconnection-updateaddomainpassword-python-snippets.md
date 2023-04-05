---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAdDomainPasswordPostRequestBody()
request_body.setAdDomainPassword('AdDomainPassword value')



await client.deviceManagement.virtualEndpoint.onPremisesConnectionsby_id('cloudPcOnPremisesConnection-id').updateAdDomainPassword.post(request_body)


```
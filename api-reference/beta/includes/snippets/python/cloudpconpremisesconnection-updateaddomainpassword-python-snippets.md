---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UpdateAdDomainPasswordPostRequestBody()
request_body.adDomainPassword = 'AdDomainPassword value'




await client.deviceManagement.virtualEndpoint.onPremisesConnections_by_id('cloudPcOnPremisesConnection-id').updateAdDomainPassword.post(request_body = request_body)


```
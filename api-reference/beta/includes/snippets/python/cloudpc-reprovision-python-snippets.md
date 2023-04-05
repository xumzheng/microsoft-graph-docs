---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReprovisionPostRequestBody()
request_body.setUserAccountType(CloudPcUserAccountType('administrator'))

request_body.setOsVersion(CloudPcOperatingSystem('windows10'))



await client.deviceManagement.virtualEndpoint.cloudPCsby_id('cloudPC-id').reprovision.post(request_body)


```
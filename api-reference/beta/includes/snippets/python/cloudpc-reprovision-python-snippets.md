---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReprovisionPostRequestBody()
request_body.UserAccountType(CloudPcUserAccountType('administrator'))

request_body.OsVersion(CloudPcOperatingSystem('windows10'))



request_configuration = ReprovisionRequestBuilderPostRequestConfiguration(
)


await client.deviceManagement.virtualEndpoint.cloudPCs_by_id('cloudPC-id').reprovision.post(request_body = request_body)


```
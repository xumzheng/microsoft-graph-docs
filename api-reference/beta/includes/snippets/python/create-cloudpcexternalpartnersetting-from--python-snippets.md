---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcExternalPartnerSetting()
request_body.set@odatatype('#microsoft.graph.cloudPcExternalPartnerSetting')

request_body.setPartnerId('198d7140-80bb-4843-8cc4-811377a49a92')

request_body.setEnableConnection(true)



result = await client.deviceManagement_virtualEndpoint_externalPartnerSettings.post(request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcExternalPartnerSetting()
request_body.set@odatatype('#microsoft.graph.cloudPcExternalPartnerSetting')

request_body.setEnableConnection(true)



result = await client.deviceManagement.virtualEndpoint.externalPartnerSettings_by_id('cloudPcExternalPartnerSetting-id').patch(request_body)


```
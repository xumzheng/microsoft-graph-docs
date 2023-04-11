---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOrganizationSettings()
request_body.@odatatype = '#microsoft.graph.cloudPcOrganizationSettings'

request_body.enableMEMAutoEnroll = true

request_body.OsVersion(CloudPcOperatingSystem('windows11'))

request_body.UserAccountType(CloudPcUserAccountType('standarduser'))

windowsSettings = CloudPcWindowsSettings()
windowsSettings.language = 'en-US'


request_body.windowsSettings = windowsSettings



result = await client.deviceManagement.virtualEndpoint.organizationSettings.patch(request_body = request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcOrganizationSettings()
request_body.@odatatype = '#microsoft.graph.cloudPcOrganizationSettings'

request_body.enable_m_e_m_auto_enroll = True

request_body.OsVersion(CloudPcOperatingSystem('windows11'))

request_body.UserAccountType(CloudPcUserAccountType('standarduser'))

windows_settings = CloudPcWindowsSettings()
windowsSettings.language = 'en-US'


request_body.windows_settings = windowsSettings



result = await client.deviceManagement.virtualEndpoint.organizationSettings.patch(request_body = request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CloudPcOrganizationSettings();
request_body.set@odatatype('#microsoft.graph.cloudPcOrganizationSettings');

request_body.setEnableMEMAutoEnroll(true);

request_body.setOsVersion(CloudPcOperatingSystem('windows11'));

request_body.setUserAccountType(CloudPcUserAccountType('standarduser'));

windowsSettings = CloudPcWindowsSettings();
windowsSettings.setLanguage('en-US');


request_body.setWindowsSettings($windowsSettings);


result = await client.deviceManagement.virtualEndpoint.organizationSettings.patch(request_body);


```
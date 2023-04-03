---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CloudPcOrganizationSettings();
requestBody.set@odatatype('#microsoft.graph.cloudPcOrganizationSettings');

requestBody.setEnableMEMAutoEnroll(true);

requestBody.setOsVersion(CloudPcOperatingSystem('windows11'));

requestBody.setUserAccountType(CloudPcUserAccountType('standarduser'));

windowsSettings = CloudPcWindowsSettings();
windowsSettings.setLanguage('en-US');


requestBody.setWindowsSettings($windowsSettings);


result = awaitclient.deviceManagement().virtualEndpoint().organizationSettings().patch(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CloudPcOrganizationSettings();
$requestBody.set@odatatype('#microsoft.graph.cloudPcOrganizationSettings');

$requestBody.setEnableMEMAutoEnroll(true);

$requestBody.setOsVersion(new CloudPcOperatingSystem('windows11'));

$requestBody.setUserAccountType(new CloudPcUserAccountType('standarduser'));

$windowsSettings = new CloudPcWindowsSettings();
$windowsSettings.setLanguage('en-US');


$requestBody.setWindowsSettings($windowsSettings);


$requestResult = $graphServiceClient.deviceManagement().virtualEndpoint().organizationSettings().patch($requestBody);


```
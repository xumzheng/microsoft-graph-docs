---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CloudPcUserSetting();
$requestBody.set@odatatype('#microsoft.graph.cloudPcUserSetting');

$requestBody.setDisplayName('Example');

$requestBody.setSelfServiceEnabled(true);

$restorePointSetting = new CloudPcRestorePointSetting();
$restorePointSetting.setFrequencyInHours(16);

$restorePointSetting.setUserRestoreEnabled(true);


$requestBody.setRestorePointSetting($restorePointSetting);
$requestBody.setLocalAdminEnabled(false);



$requestResult = $graphServiceClient.deviceManagement().virtualEndpoint().userSettingsById('cloudPcUserSetting-id').patch($requestBody);


```
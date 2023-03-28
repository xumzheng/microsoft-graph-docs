---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new CloudPcUserSettingRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPcUserSettingRequestBuilderGetQueryParameters();
$queryParameters->expand = ["assignments"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->deviceManagement()->virtualEndpoint()->userSettingsById('cloudPcUserSetting-id')->get($requestConfiguration);


```
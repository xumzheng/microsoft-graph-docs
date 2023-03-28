---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new DeviceRequestBuilderGetRequestConfiguration();

$queryParameters = new DeviceRequestBuilderGetQueryParameters();
$queryParameters->select = ["id","extensionAttributes"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->devicesById('device-id')->get($requestConfiguration);


```
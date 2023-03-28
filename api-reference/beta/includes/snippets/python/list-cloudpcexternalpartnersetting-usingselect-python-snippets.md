---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ExternalPartnerSettingsRequestBuilderGetRequestConfiguration();

$queryParameters = new ExternalPartnerSettingsRequestBuilderGetQueryParameters();
$queryParameters->select = ["id","partnerId","enableConnection"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->deviceManagement()->virtualEndpoint()->externalPartnerSettings()->get($requestConfiguration);


```
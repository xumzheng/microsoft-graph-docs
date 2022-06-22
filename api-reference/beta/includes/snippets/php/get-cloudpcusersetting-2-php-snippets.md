---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CloudPcUserSettingRequestBuilderGetRequestConfiguration();

$queryParameters = new CloudPcUserSettingRequestBuilderGetQueryParameters();
$queryParameters->expand = 'assignments';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->deviceManagement()->virtualEndpoint()->userSettingsById('cloudPcUserSetting-id')->get($requestConfiguration);


```
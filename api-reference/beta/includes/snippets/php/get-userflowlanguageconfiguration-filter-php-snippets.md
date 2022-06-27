---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new LanguagesRequestBuilderGetRequestConfiguration();

$queryParameters = new LanguagesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'isEnabled%20eq%20true';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->languages()->get($requestConfiguration);


```
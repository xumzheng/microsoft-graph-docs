---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new B2xUserFlowsRequestBuilderGetRequestConfiguration();

$queryParameters = new B2xUserFlowsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'identityProviders';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->b2xUserFlows()->get($requestConfiguration);


```
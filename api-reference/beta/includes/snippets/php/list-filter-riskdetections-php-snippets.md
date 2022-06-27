---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new RiskDetectionsRequestBuilderGetRequestConfiguration();

$queryParameters = new RiskDetectionsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'riskEventType%20eq%20\'unfamiliarFeatures\'%20or%20riskLevel%20eq%20\'medium\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityProtection()->riskDetections()->get($requestConfiguration);


```
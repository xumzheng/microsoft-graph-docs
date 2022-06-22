---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ServicePrincipalRiskDetectionsRequestBuilderGetRequestConfiguration();

$queryParameters = new ServicePrincipalRiskDetectionsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'riskEventType%20eq%20\'investigationsThreatIntelligence\'%20or%20riskLevel%20eq%20\'medium\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityProtection()->servicePrincipalRiskDetections()->get($requestConfiguration);


```
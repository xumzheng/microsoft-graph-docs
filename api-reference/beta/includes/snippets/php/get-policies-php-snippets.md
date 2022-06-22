---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new PoliciesRequestBuilderGetRequestConfiguration();

$queryParameters = new PoliciesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'displayName%20eq%20\'SimplePolicy1\'%20or%20displayName%20eq%20\'SimplePolicy2\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->conditionalAccess()->policies()->get($requestConfiguration);


```
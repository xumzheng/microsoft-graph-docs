---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new CustomSecurityAttributeDefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new CustomSecurityAttributeDefinitionsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'attributeSet%20eq%20\'Engineering\'%20and%20status%20eq%20\'Available\'%20and%20type%20eq%20\'String\'';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->directory()->customSecurityAttributeDefinitions()->get($requestConfiguration);


```
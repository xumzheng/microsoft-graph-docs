---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ContactsRequestBuilderGetRequestConfiguration();

$queryParameters = new ContactsRequestBuilderGetQueryParameters();
$queryParameters->select = 'displayName,emailAddresses';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->contacts()->get($requestConfiguration);


```
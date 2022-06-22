---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new TeamsRequestBuilderGetRequestConfiguration();

$queryParameters = new TeamsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'displayName%20eq%20\'A%20Contoso%20Team\'';
$queryParameters->select = 'id,description';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->teams()->get($requestConfiguration);


```
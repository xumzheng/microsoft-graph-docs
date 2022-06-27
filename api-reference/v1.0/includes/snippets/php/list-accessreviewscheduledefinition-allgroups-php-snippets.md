---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DefinitionsRequestBuilderGetRequestConfiguration();

$queryParameters = new DefinitionsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'contains(scope/microsoft.graph.accessReviewQueryScope/query,%20\'./members\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->get($requestConfiguration);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'Extensions/any';
$queryParameters->expand = 'Extensions($filter=id%20eq%20\'Com.Contoso.Referral\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->messages()->get($requestConfiguration);


```
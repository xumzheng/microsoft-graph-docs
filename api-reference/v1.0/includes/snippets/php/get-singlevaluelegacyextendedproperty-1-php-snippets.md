---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessageRequestBuilderGetRequestConfiguration();

$queryParameters = new MessageRequestBuilderGetQueryParameters();
$queryParameters->expand = 'singleValueExtendedProperties($filter=id%20eq%20\'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->messagesById('message-id')->get($requestConfiguration);


```
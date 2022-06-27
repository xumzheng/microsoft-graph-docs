---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessageRequestBuilderGetRequestConfiguration();

$queryParameters = new MessageRequestBuilderGetQueryParameters();
$queryParameters->expand = 'mentions';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->messagesById('message-id')->get($requestConfiguration);


```
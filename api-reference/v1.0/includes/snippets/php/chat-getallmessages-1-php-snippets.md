---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GetAllMessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new GetAllMessagesRequestBuilderGetQueryParameters();
$queryParameters->top = 2;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->usersById('user-id')->chats()->getAllMessages()()->get($requestConfiguration);


```
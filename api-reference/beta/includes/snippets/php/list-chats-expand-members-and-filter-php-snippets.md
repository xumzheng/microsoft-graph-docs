---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ChatsRequestBuilderGetRequestConfiguration();

$queryParameters = new ChatsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'members';
$queryParameters->filter = 'members/any';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->usersById('user-id')->chats()->get($requestConfiguration);


```
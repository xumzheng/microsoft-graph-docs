---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new MessagesRequestBuilderGetRequestConfiguration();

$queryParameters = new MessagesRequestBuilderGetQueryParameters();
$queryParameters->filter = 'MentionsPreview/IsMentioned%20eq%20true';
$queryParameters->select = 'Subject,Sender,ReceivedDateTime,MentionsPreview';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->messages()->get($requestConfiguration);


```
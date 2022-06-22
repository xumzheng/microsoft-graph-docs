---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AttachmentRequestBuilderGetRequestConfiguration();

$queryParameters = new AttachmentRequestBuilderGetQueryParameters();
$queryParameters->expand = 'microsoft.graph.itemattachment/item';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->messagesById('message-id')->attachmentsById('attachment-id')->get($requestConfiguration);


```
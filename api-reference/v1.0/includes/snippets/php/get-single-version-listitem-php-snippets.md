---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ListItemVersionRequestBuilderGetRequestConfiguration();

$queryParameters = new ListItemVersionRequestBuilderGetQueryParameters();
$queryParameters->expand = 'fields';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sitesById('site-id')->listsById('list-id')->itemsById('listItem-id')->versionsById('listItemVersion-id')->get($requestConfiguration);


```
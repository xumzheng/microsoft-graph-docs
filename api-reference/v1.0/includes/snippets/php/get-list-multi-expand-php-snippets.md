---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ListRequestBuilderGetRequestConfiguration();

$queryParameters = new ListRequestBuilderGetQueryParameters();
$queryParameters->select = 'id,name,lastModifiedDateTime';
$queryParameters->expand = 'columns(select=name,description),items)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->sitesById('site-id')->listsById('list-id')->get($requestConfiguration);


```
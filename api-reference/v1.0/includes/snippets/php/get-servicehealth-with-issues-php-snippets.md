---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new ServiceHealthRequestBuilderGetRequestConfiguration();

$queryParameters = new ServiceHealthRequestBuilderGetQueryParameters();
$queryParameters->expand = 'issues';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->admin()->serviceAnnouncement()->healthOverviewsById('serviceHealth-id')->get($requestConfiguration);


```
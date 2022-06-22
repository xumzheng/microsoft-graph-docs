---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new HealthOverviewsRequestBuilderGetRequestConfiguration();

$queryParameters = new HealthOverviewsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'issues';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->admin()->serviceAnnouncement()->healthOverviews()->get($requestConfiguration);


```
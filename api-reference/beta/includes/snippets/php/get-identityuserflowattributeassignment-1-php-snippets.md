---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new UserAttributeAssignmentsRequestBuilderGetRequestConfiguration();

$queryParameters = new UserAttributeAssignmentsRequestBuilderGetQueryParameters();

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->b2cUserFlowsById('b2cIdentityUserFlow-id')->userAttributeAssignments()->get($requestConfiguration);


```
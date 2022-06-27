---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration();

$queryParameters = new IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters();
$queryParameters->expand = 'userAttribute';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identity()->b2xUserFlowsById('b2xIdentityUserFlow-id')->userAttributeAssignmentsById('identityUserFlowAttributeAssignment-id')->get($requestConfiguration);


```
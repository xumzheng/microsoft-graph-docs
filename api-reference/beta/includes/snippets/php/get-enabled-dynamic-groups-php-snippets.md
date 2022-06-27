---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new GroupsRequestBuilderGetRequestConfiguration();

$queryParameters = new GroupsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT)%20and%20membershipRuleProcessingState%20eq%20\'On\'';
$queryParameters->count = true;
$queryParameters->select = 'id,membershipRule,membershipRuleProcessingState';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->groups()->get($requestConfiguration);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessPackageAssignmentRequestsRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessPackageAssignmentRequestsRequestBuilderGetQueryParameters();
$queryParameters->expand = 'requestor($expand=connectedOrganization)';
$queryParameters->filter = '(requestState%20eq%20\'PendingApproval\')';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageAssignmentRequests()->get($requestConfiguration);


```
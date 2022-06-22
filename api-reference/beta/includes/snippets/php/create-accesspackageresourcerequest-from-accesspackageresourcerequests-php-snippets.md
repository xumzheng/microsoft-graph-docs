---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRequest();


$requestRequestBody->setCatalogId('26ac0c0a-08bc-4a7b-a313-839f58044ba5');
$requestRequestBody->setRequestType('AdminAdd');
$requestRequestBody->setJustification('');

$accessPackageResource = new AccessPackageResource();
$requestRequestBody->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setDisplayName('Sales');
$accessPackageResource->setDescription('https://contoso.sharepoint.com/sites/Sales');
$accessPackageResource->setUrl('https://contoso.sharepoint.com/sites/Sales');
$accessPackageResource->setResourceType('SharePoint Online Site');
$accessPackageResource->setOriginId('https://contoso.sharepoint.com/sites/Sales');
$accessPackageResource->setOriginSystem('SharePointOnline');

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceRequests()->post($requestRequestBody);


```
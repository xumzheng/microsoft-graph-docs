---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessPackageResourceRequest();


$requestRequestBody->setCatalogId('de9315c1-272b-4905-924b-cc112ca180c7');

$accessPackageResource = new AccessPackageResource();
$requestRequestBody->setAccessPackageResource($accessPackageResource);


$accessPackageResource->setDisplayName('Community Outreach');
$accessPackageResource->setDescription('https://contoso.sharepoint.com/sites/CSR');
$accessPackageResource->setResourceType('SharePoint Online Site');
$accessPackageResource->setOriginId('https://contoso.sharepoint.com/sites/CSR');
$accessPackageResource->setOriginSystem('SharePointOnline');
$accessPackageResourceAdditionalData = [
	"accessPackageResourceEnvironment@odata.bind" => 'accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57',
];
$accessPackageResource->setAdditionalData($accessPackageResourceAdditionalData);

$requestRequestBody->setRequestType('AdminAdd');
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceRequests()->post($requestRequestBody);


```
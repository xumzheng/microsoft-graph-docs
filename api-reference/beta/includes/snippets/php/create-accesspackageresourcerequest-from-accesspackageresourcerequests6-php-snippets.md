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


$accessPackageResource->setDisplayName('Faculty cafeteria ordering');
$accessPackageResource->setDescription('Example application');
$accessPackageResource->setUrl('https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/');
$accessPackageResource->setResourceType('Application');
$accessPackageResource->setOriginId('2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e');
$accessPackageResource->setOriginSystem('AadApplication');
$attributesArray = [];

$attributes1 = new AccessPackageResourceAttribute();

$attributes1->setAttributeName('extension_2b676109c7c74ae2b41549205f1947ed_personalTitle');
$attributes1->setIsEditable(True);
$attributes1->setIsPersistedOnAssignmentRemoval(True);

$attributeSource = new AccessPackageResourceAttributeSource();
$attributes1->setAttributeSource($attributeSource);


$attributeSourceAdditionalData = [
		"@odata.type" => '#microsoft.graph.accessPackageResourceAttributeQuestion',
	];
$attributeSource->setAdditionalData($attributeSourceAdditionalData);


$attributeDestination = new AccessPackageResourceAttributeDestination();
$attributes1->setAttributeDestination($attributeDestination);


$attributeDestinationAdditionalData = [
	"@odata.type" => '#microsoft.graph.accessPackageUserDirectoryAttributeStore',
];
$attributeDestination->setAdditionalData($attributeDestinationAdditionalData);


$attributesArray []= $attributes1;
$accessPackageResource->setAttributes($attributesArray);

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageResourceRequests()->post($requestRequestBody);


```
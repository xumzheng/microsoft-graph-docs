---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomAccessPackageWorkflowExtension-idPutRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.customAccessPackageWorkflowExtension',
	"displayName" => 'test_action_0124_email',
	"description" => 'this is for graph testing only',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->customAccessPackageWorkflowExtensionsById('customAccessPackageWorkflowExtension-id')->put($requestRequestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CustomAccessPackageWorkflowExtension();


$requestRequestBody->setDisplayName('test_action_0124');
$requestRequestBody->setDescription('this is for graph testing only');

$endpointConfiguration = new CustomExtensionEndpointConfiguration();
$requestRequestBody->setEndpointConfiguration($endpointConfiguration);


$endpointConfigurationAdditionalData = [
	"@odata.type" => '#microsoft.graph.logicAppTriggerEndpointConfiguration',
	"subscriptionId" => '38ab2ccc-3747-4567-b36b-9478f5602f0d',
	"resourceGroupName" => 'EMLogicApp',
	"logicAppWorkflowName" => 'customextension_test',
];
$endpointConfiguration->setAdditionalData($endpointConfigurationAdditionalData);


$authenticationConfiguration = new CustomExtensionAuthenticationConfiguration();
$requestRequestBody->setAuthenticationConfiguration($authenticationConfiguration);


$authenticationConfigurationAdditionalData = [
"@odata.type" => '#microsoft.graph.azureAdTokenAuthentication',
"resourceId" => 'f604bd15-f785-4309-ad7c-6fad18ddb6cb',
];
$authenticationConfiguration->setAdditionalData($authenticationConfigurationAdditionalData);

$result =  $graphClient->identityGovernance()->entitlementManagement()->accessPackageCatalogsById('accessPackageCatalog-id')->customAccessPackageWorkflowExtensions()->post($requestRequestBody);


```
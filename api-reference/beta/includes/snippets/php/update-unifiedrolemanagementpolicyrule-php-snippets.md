---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedRoleManagementPolicyRule();


$requestRequestBody->setId('Expiration_EndUser_Assignment');

$target = new UnifiedRoleManagementPolicyRuleTarget();
$requestRequestBody->setTarget($target);


$target->setCaller('EndUser');
$target->setOperations( [
'All',],
$target->setLevel('Assignment');
$target->setInheritableSettings( [
],
$target->setEnforcedSettings( [
],
$targetAdditionalData = [
	"@odata.type" => 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget',
];
$target->setAdditionalData($targetAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.unifiedRoleManagementPolicyExpirationRule',
"isExpirationRequired" => True,
"maximumDuration" => 'PT1H45M',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->roleManagementPoliciesById('unifiedRoleManagementPolicy-id')->rulesById('unifiedRoleManagementPolicyRule-id')->patch($requestRequestBody);


```
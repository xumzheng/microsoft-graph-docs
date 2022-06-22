---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CrossTenantAccessPolicyConfigurationDefault();



$b2bCollaborationOutbound = new CrossTenantAccessPolicyB2BSetting();
$requestRequestBody->setB2bCollaborationOutbound($b2bCollaborationOutbound);



$usersAndGroups = new CrossTenantAccessPolicyTargetConfiguration();
$b2bCollaborationOutbound->setUsersAndGroups($usersAndGroups);


$usersAndGroups->setAccessType(new CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'));
$targetsArray = [];

$targets1 = new CrossTenantAccessPolicyTarget();

$targets1->setTarget('0be493dc-cb56-4a53-936f-9cf64410b8b0');
$targets1->setTargetType(new CrossTenantAccessPolicyTargetType('group'));

$targetsArray []= $targets1;
$usersAndGroups->setTargets($targetsArray);


$applications = new CrossTenantAccessPolicyTargetConfiguration();
$b2bCollaborationOutbound->setApplications($applications);


$applications->setAccessType(new CrossTenantAccessPolicyTargetConfigurationAccessType('blocked'));
$targetsArray = [];

$targets1 = new CrossTenantAccessPolicyTarget();

$targets1->setTarget('AllApplications');
$targets1->setTargetType(new CrossTenantAccessPolicyTargetType('application'));

$targetsArray []= $targets1;
$applications->setTargets($targetsArray);


$result =  $graphClient->policies()->crossTenantAccessPolicy()->default()->patch($requestRequestBody);


```
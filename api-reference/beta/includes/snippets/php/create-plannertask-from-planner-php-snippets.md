---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerTask();


$requestRequestBody->setPlanId('xqQg5FS2LkCp935s-FIFm2QAFkHM');
$requestRequestBody->setBucketId('hsOf2dhOJkqyYYZEtdzDe2QAIUCR');
$requestRequestBody->setTitle('Update client list');

$assignments = new PlannerAssignments();
$requestRequestBody->setAssignments($assignments);


$assignmentsAdditionalData = [
];
$assignments->setAdditionalData($assignmentsAdditionalData);

$result =  $graphClient->planner()->tasks()->post($requestRequestBody);


```
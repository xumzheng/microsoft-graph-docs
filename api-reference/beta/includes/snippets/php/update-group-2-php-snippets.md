---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$assignedLabelsArray = [];

$assignedLabels1 = new AssignedLabel();

$assignedLabels1->setLabelId('45cd0c48-c540-4358-ad79-a3658cdc5b88');

$assignedLabelsArray []= $assignedLabels1;
$requestRequestBody->setAssignedLabels($assignedLabelsArray);
$result =  $graphClient->groupsById('group-id')->patch($requestRequestBody);


```
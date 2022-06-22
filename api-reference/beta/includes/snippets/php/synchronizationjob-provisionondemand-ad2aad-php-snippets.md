---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ParametersRequestBody();


$parametersArray = [];

$parameters1 = new SynchronizationJobApplicationParameters();

$parameters1->setRuleId('6c409270-f78a-4bc6-af23-7cf3ab6482fe');
$subjectsArray = [];

$subjects1 = new SynchronizationJobSubject();

$subjects1->setObjectId('CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com');
$subjects1->setObjectTypeName('user');

$subjectsArray []= $subjects1;
$parameters1->setSubjects($subjectsArray);

$parametersArray []= $parameters1;
$requestRequestBody->setParameters($parametersArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->provisionOnDemand()->post($requestRequestBody);


```
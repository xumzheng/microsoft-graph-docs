---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ParametersRequestBody();


$parametersArray = [];

$parameters1 = new SynchronizationJobApplicationParameters();

$subjectsArray = [];

$subjects1 = new SynchronizationJobSubject();

$subjects1->setObjectId('9bb0f679-a883-4a6f-8260-35b491b8b8c8');
$subjects1->setObjectTypeName('User');

$subjectsArray []= $subjects1;
$parameters1->setSubjects($subjectsArray);
$parameters1->setRuleId('ea807875-5618-4f0a-9125-0b46a05298ca');

$parametersArray []= $parameters1;
$requestRequestBody->setParameters($parametersArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->provisionOnDemand()->post($requestRequestBody);


```
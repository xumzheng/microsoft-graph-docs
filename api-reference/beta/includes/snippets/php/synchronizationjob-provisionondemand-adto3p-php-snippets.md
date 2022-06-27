---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ParametersRequestBody();


$parametersArray = [];

$parametersparameters1 = new SynchronizationJobApplicationParameters();

$subjectsArray = [];

$subjectssubjects1 = new SynchronizationJobSubject();

$subjectssubjects1->setObjectId('9bb0f679-a883-4a6f-8260-35b491b8b8c8');
$subjectssubjects1->setObjectTypeName('User');

$subjectsArray []= $subjectssubjects1;
$parametersparameters1->setSubjects($subjectsArray);
$parametersparameters1->setRuleId('ea807875-5618-4f0a-9125-0b46a05298ca');

$parametersArray []= $parametersparameters1;
$requestRequestBody->setParameters($parametersArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->provisionOnDemand()->post($requestRequestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ParametersRequestBody();


$parametersArray = [];

$parametersparameters1 = new SynchronizationJobApplicationParameters();

$parametersparameters1->setRuleId('6c409270-f78a-4bc6-af23-7cf3ab6482fe');
$subjectsArray = [];

$subjectssubjects1 = new SynchronizationJobSubject();

$subjectssubjects1->setObjectId('CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com');
$subjectssubjects1->setObjectTypeName('user');

$subjectsArray []= $subjectssubjects1;
$parametersparameters1->setSubjects($subjectsArray);

$parametersArray []= $parametersparameters1;
$requestRequestBody->setParameters($parametersArray);
$result =  $graphClient->servicePrincipalsById('servicePrincipal-id')->synchronization()->jobsById('synchronizationJob-id')->provisionOnDemand()->post($requestRequestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ProjectParticipation();
$requestBody->setAllowedAudiences(new AllowedAudiences('organization'));

$client = new CompanyDetail();
$client->setDepartment('Corporate Marketing');

$client->setWebUrl('https://www.contoso.com');


$requestBody->setClient($client);


$requestResult = $graphServiceClient->me()->profile()->projectsById('projectParticipation-id')->patch($requestBody);


```
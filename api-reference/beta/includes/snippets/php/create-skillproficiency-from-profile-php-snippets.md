---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SkillProficiency();


$requestRequestBody->setCategories( [
'Professional',],
$requestRequestBody->setAllowedAudiences(new AllowedAudiences('organization'));
$requestRequestBody->setDisplayName('API Design');
$requestRequestBody->setProficiency(new SkillProficiencyLevel('generalProfessional'));
$requestRequestBody->setCollaborationTags( [
'ableToMentor',],
$result =  $graphClient->me()->profile()->skills()->post($requestRequestBody);


```
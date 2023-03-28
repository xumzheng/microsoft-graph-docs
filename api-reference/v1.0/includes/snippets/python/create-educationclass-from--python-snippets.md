---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new EducationClass();
$requestBody.set@odatatype('#microsoft.graph.educationClass');

$requestBody.setDisplayName('String');

$requestBody.setMailNickname('String');

$requestBody.setDescription('String');

$createdBy = new IdentitySet();
$createdBy.set@odatatype('microsoft.graph.identitySet');


$requestBody.setCreatedBy($createdBy);
$requestBody.setClassCode('String');

$requestBody.setExternalName('String');

$requestBody.setExternalId('String');

$requestBody.setExternalSource(new EducationExternalSource('string'));

$requestBody.setExternalSourceDetail('String');

$requestBody.setGrade('String');

$term = new EducationTerm();
$term.set@odatatype('microsoft.graph.educationTerm');


$requestBody.setTerm($term);


$requestResult = $graphServiceClient.education().classes().post($requestBody);


```
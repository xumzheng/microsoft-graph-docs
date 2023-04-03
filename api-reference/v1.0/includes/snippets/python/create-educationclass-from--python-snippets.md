---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationClass();
requestBody.set@odatatype('#microsoft.graph.educationClass');

requestBody.setDisplayName('String');

requestBody.setMailNickname('String');

requestBody.setDescription('String');

createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);
requestBody.setClassCode('String');

requestBody.setExternalName('String');

requestBody.setExternalId('String');

requestBody.setExternalSource(EducationExternalSource('string'));

requestBody.setExternalSourceDetail('String');

requestBody.setGrade('String');

term = EducationTerm();
term.set@odatatype('microsoft.graph.educationTerm');


requestBody.setTerm($term);


result = awaitclient.education().classes().post(requestBody);


```
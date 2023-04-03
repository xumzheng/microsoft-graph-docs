---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationClass();
requestBody.setDescription('Health Level 1');

requestBody.setClassCode('Health 501');

requestBody.setDisplayName('Health 1');

requestBody.setExternalId('11019');

requestBody.setExternalName('Health Level 1');

requestBody.setExternalSource(EducationExternalSource('sis'));

requestBody.setMailNickname('fineartschool.net');



result = await client.education().classes().post(requestBody);


```
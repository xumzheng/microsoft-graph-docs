---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonCertification();
requestBody.setIssuingAuthority('International Academy of Marketing Excellence');

requestBody.setIssuingCompany('International Academy of Marketing Excellence');



result = await client.usersById('user-id').profile().certificationsById('personCertification-id').patch(requestBody);


```
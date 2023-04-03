---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonCertification();
requestBody.setIssuingAuthority('International Academy of Marketing Excellence');

requestBody.setIssuingCompany('International Academy of Marketing Excellence');



result = awaitclient.usersById('user-id').profile().certificationsById('personCertification-id').patch(requestBody);


```
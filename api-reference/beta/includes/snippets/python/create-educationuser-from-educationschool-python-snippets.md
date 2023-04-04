---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReferenceCreate();
request_body.set@odataid('https://graph.microsoft.com/beta/education/users/14008');



await client.education.schoolsById('educationSchool-id').users.ref.post(request_body);


```
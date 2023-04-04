---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationUser();
request_body.setDisplayName('Rogelio Cazares');

request_body.setGivenName('Rogelio');

request_body.setMiddleName('Fernando');

request_body.setSurname('Cazares');



result = await client.education.usersById('educationUser-id').patch(request_body);


```
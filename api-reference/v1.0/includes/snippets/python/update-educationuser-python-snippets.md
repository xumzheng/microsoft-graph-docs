---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationUser();
requestBody.setDisplayName('Rogelio Cazares');

requestBody.setGivenName('Rogelio');

requestBody.setMiddleName('Fernando');

requestBody.setSurname('Cazares');



result = awaitclient.education().usersById('educationUser-id').patch(requestBody);


```
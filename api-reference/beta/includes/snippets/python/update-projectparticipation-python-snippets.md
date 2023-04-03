---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ProjectParticipation();
requestBody.setAllowedAudiences(AllowedAudiences('organization'));

client = CompanyDetail();
client.setDepartment('Corporate Marketing');

client.setWebUrl('https://www.contoso.com');


requestBody.setClient($client);


result = awaitclient.me().profile().projectsById('projectParticipation-id').patch(requestBody);


```
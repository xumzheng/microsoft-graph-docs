---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ProvisionOnDemandPostRequestBody();
parametersSynchronizationJobApplicationParameters1 = SynchronizationJobApplicationParameters();
parametersSynchronizationJobApplicationParameters1.setRuleId('6c409270-f78a-4bc6-af23-7cf3ab6482fe');

subjectsSynchronizationJobSubject1 = SynchronizationJobSubject();
subjectsSynchronizationJobSubject1.setObjectId('CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com');

subjectsSynchronizationJobSubject1.setObjectTypeName('user');


subjectsArray []= subjectsSynchronizationJobSubject1;
parametersSynchronizationJobApplicationParameters1.setSubjects(subjectsArray);



parametersArray []= parametersSynchronizationJobApplicationParameters1;
requestBody.setParameters(parametersArray);




result = await client.servicePrincipalsById('servicePrincipal-id').synchronization().jobsById('synchronizationJob-id').provisionOnDemand().post(requestBody);


```
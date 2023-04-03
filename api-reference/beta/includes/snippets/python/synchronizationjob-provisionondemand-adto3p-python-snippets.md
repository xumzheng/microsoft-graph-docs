---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ProvisionOnDemandPostRequestBody();
parametersSynchronizationJobApplicationParameters1 = SynchronizationJobApplicationParameters();
subjectsSynchronizationJobSubject1 = SynchronizationJobSubject();
subjectsSynchronizationJobSubject1.setObjectId('9bb0f679-a883-4a6f-8260-35b491b8b8c8');

subjectsSynchronizationJobSubject1.setObjectTypeName('User');


subjectsArray []= subjectsSynchronizationJobSubject1;
parametersSynchronizationJobApplicationParameters1.setSubjects(subjectsArray);


parametersSynchronizationJobApplicationParameters1.setRuleId('ea807875-5618-4f0a-9125-0b46a05298ca');


parametersArray []= parametersSynchronizationJobApplicationParameters1;
requestBody.setParameters(parametersArray);




result = awaitclient.servicePrincipalsById('servicePrincipal-id').synchronization().jobsById('synchronizationJob-id').provisionOnDemand().post(requestBody);


```
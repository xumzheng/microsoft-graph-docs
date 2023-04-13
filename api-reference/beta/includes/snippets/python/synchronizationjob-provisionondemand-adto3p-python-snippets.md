---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProvisionOnDemandPostRequestBody()
parameters_synchronization_job_application_parameters1 = SynchronizationJobApplicationParameters()
subjects_synchronization_job_subject1 = SynchronizationJobSubject()
subjectsSynchronizationJobSubject1.objectId = '9bb0f679-a883-4a6f-8260-35b491b8b8c8'

subjectsSynchronizationJobSubject1.objectTypeName = 'User'


subjectsArray []= subjectsSynchronizationJobSubject1;
parametersSynchronizationJobApplicationParameters1.subjects(subjectsArray)


parametersSynchronizationJobApplicationParameters1.ruleId = 'ea807875-5618-4f0a-9125-0b46a05298ca'


parametersArray []= parametersSynchronizationJobApplicationParameters1;
request_body.parameters(parametersArray)





result = await client.servicePrincipals_by_id('servicePrincipal-id').synchronization.jobs_by_id('synchronizationJob-id').provisionOnDemand.post(request_body = request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ProvisionOnDemandPostRequestBody()
parameters_synchronization_job_application_parameters1 = SynchronizationJobApplicationParameters()
parametersSynchronizationJobApplicationParameters1.ruleId = '33f7c90d-bf71-41b1-bda6-aaf0ddbee5d8#V2'

subjects_synchronization_job_subject1 = SynchronizationJobSubject()
subjectsSynchronizationJobSubject1.objectId = '8213fd99-d6b6-417b-8e13-af6334856215'

subjectsSynchronizationJobSubject1.objectTypeName = 'Group'

subjects_synchronization_job_subject1_links = SynchronizationLinkedObjects()
members_synchronization_job_subject1 = SynchronizationJobSubject()
membersSynchronizationJobSubject1.objectId = 'cbc86211-6ada-4803-b73f-8039cf56d8a2'

membersSynchronizationJobSubject1.objectTypeName = 'User'


membersArray []= membersSynchronizationJobSubject1;
members_synchronization_job_subject2 = SynchronizationJobSubject()
membersSynchronizationJobSubject2.objectId = '2bc86211-6ada-4803-b73f-8039cf56d8a2'

membersSynchronizationJobSubject2.objectTypeName = 'User'


membersArray []= membersSynchronizationJobSubject2;
subjectsSynchronizationJobSubject1Links.members(membersArray)



subjectsSynchronizationJobSubject1.links = subjectsSynchronizationJobSubject1Links

subjectsArray []= subjectsSynchronizationJobSubject1;
parametersSynchronizationJobApplicationParameters1.subjects(subjectsArray)



parametersArray []= parametersSynchronizationJobApplicationParameters1;
request_body.parameters(parametersArray)





result = await client.servicePrincipals_by_id('servicePrincipal-id').synchronization.jobs_by_id('synchronizationJob-id').provisionOnDemand.post(request_body = request_body)


```
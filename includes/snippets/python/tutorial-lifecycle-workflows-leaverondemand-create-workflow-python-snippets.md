---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.setCategory(LifecycleWorkflowCategory('leaver'))

request_body.setDisplayName('Real-time employee termination')

request_body.setDescription('Execute real-time termination tasks for employees on their last day of work')

request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(false)

executionConditions = WorkflowExecutionConditions()
executionConditions.set@odatatype('#microsoft.graph.identityGovernance.onDemandExecutionOnly')


request_body.setExecutionConditions($executionConditions)
tasksTask1 = Task()
tasksTask1.setContinueOnError(false)

tasksTask1.setDescription('Remove user from all Azure AD groups memberships')

tasksTask1.setDisplayName('Remove user from all groups')

tasksTask1.setExecutionSequence(1)

tasksTask1.setIsEnabled(true)

tasksTask1.setTaskDefinitionId('b3a31406-2a15-4c9a-b25b-a658fa5f07fc')

tasksTask1.setArguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.setContinueOnError(false)

tasksTask2.setDescription('Remove user from all Teams memberships')

tasksTask2.setDisplayName('Remove user from all Teams')

tasksTask2.setExecutionSequence(2)

tasksTask2.setIsEnabled(true)

tasksTask2.setTaskDefinitionId('81f7b200-2816-4b3b-8c5d-dc556f07b024')

tasksTask2.setArguments([])


tasksArray []= tasksTask2;
tasksTask3 = Task()
tasksTask3.setContinueOnError(false)

tasksTask3.setDescription('Delete user account in Azure AD')

tasksTask3.setDisplayName('Delete User Account')

tasksTask3.setExecutionSequence(3)

tasksTask3.setIsEnabled(true)

tasksTask3.setTaskDefinitionId('8d18588d-9ad3-4c0f-99d0-ec215f0e3dff')

tasksTask3.setArguments([])


tasksArray []= tasksTask3;
request_body.setTasks(tasksArray)



request_config = WorkflowsRequestBuilderPostRequestConfiguration(
request_config = WorkflowsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body, headers=)


```
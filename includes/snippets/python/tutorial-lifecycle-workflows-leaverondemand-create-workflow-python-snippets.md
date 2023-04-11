---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.Category(LifecycleWorkflowCategory('leaver'))

request_body.displayName = 'Real-time employee termination'

request_body.description = 'Execute real-time termination tasks for employees on their last day of work'

request_body.isEnabled = true

request_body.isSchedulingEnabled = false

executionConditions = WorkflowExecutionConditions()
executionConditions.@odatatype = '#microsoft.graph.identityGovernance.onDemandExecutionOnly'


request_body.executionConditions = executionConditions
tasksTask1 = Task()
tasksTask1.continueOnError = false

tasksTask1.description = 'Remove user from all Azure AD groups memberships'

tasksTask1.displayName = 'Remove user from all groups'

tasksTask1.executionSequence = 1

tasksTask1.isEnabled = true

tasksTask1.taskDefinitionId = 'b3a31406-2a15-4c9a-b25b-a658fa5f07fc'

tasksTask1.Arguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.continueOnError = false

tasksTask2.description = 'Remove user from all Teams memberships'

tasksTask2.displayName = 'Remove user from all Teams'

tasksTask2.executionSequence = 2

tasksTask2.isEnabled = true

tasksTask2.taskDefinitionId = '81f7b200-2816-4b3b-8c5d-dc556f07b024'

tasksTask2.Arguments([])


tasksArray []= tasksTask2;
tasksTask3 = Task()
tasksTask3.continueOnError = false

tasksTask3.description = 'Delete user account in Azure AD'

tasksTask3.displayName = 'Delete User Account'

tasksTask3.executionSequence = 3

tasksTask3.isEnabled = true

tasksTask3.taskDefinitionId = '8d18588d-9ad3-4c0f-99d0-ec215f0e3dff'

tasksTask3.Arguments([])


tasksArray []= tasksTask3;
request_body.tasks(tasksArray)





result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body = request_body)


```
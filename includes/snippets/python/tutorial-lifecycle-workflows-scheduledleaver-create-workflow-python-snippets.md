---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.Category(LifecycleWorkflowCategory('leaver'))

request_body.displayName = 'Post-Offboarding of an employee'

request_body.description = 'Configure offboarding tasks for employees after their last day of work'

request_body.isEnabled = true

request_body.isSchedulingEnabled = false

executionConditions = WorkflowExecutionConditions()
executionConditions.@odatatype = '#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => executionConditions = Scope()
		executionConditions.@odatatype = '#microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		executionConditions.rule = 'department eq \'Marketing\''


executionConditions.scope = scope

'trigger' => executionConditions = Trigger()
		executionConditions.@odatatype = '#microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		executionConditions.timeBasedAttribute = 'employeeLeaveDateTime'

		executionConditions.offsetInDays = 7


executionConditions.trigger = trigger

];
executionConditions.additionaldata(additionalData)



request_body.executionConditions = executionConditions
tasksTask1 = Task()
tasksTask1.Category(LifecycleTaskCategory('leaver'))

tasksTask1.continueOnError = false

tasksTask1.description = 'Remove all licenses assigned to the user'

tasksTask1.displayName = 'Remove all licenses for user'

tasksTask1.executionSequence = 1

tasksTask1.isEnabled = true

tasksTask1.taskDefinitionId = '8fa97d28-3e52-4985-b3a9-a1126f9b8b4e'

tasksTask1.Arguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.Category(LifecycleTaskCategory('leaver'))

tasksTask2.continueOnError = false

tasksTask2.description = 'Remove user from all Teams memberships'

tasksTask2.displayName = 'Remove user from all Teams'

tasksTask2.executionSequence = 2

tasksTask2.isEnabled = true

tasksTask2.taskDefinitionId = '81f7b200-2816-4b3b-8c5d-dc556f07b024'

tasksTask2.Arguments([])


tasksArray []= tasksTask2;
tasksTask3 = Task()
tasksTask3.Category(LifecycleTaskCategory('leaver'))

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
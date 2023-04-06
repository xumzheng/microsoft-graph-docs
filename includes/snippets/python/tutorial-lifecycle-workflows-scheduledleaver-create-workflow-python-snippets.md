---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.setCategory(LifecycleWorkflowCategory('leaver'))

request_body.setDisplayName('Post-Offboarding of an employee')

request_body.setDescription('Configure offboarding tasks for employees after their last day of work')

request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(false)

executionConditions = WorkflowExecutionConditions()
executionConditions.set@odatatype('#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions')

additionalData = [
'scope' => executionConditions = Scope()
		executionConditions.set@odatatype('#microsoft.graph.identityGovernance.ruleBasedSubjectSet')

		executionConditions.setRule('department eq \'Marketing\'')


executionConditions.setScope($scope)

'trigger' => executionConditions = Trigger()
		executionConditions.set@odatatype('#microsoft.graph.identityGovernance.timeBasedAttributeTrigger')

		executionConditions.setTimeBasedAttribute('employeeLeaveDateTime')

		executionConditions.setOffsetInDays(7)


executionConditions.setTrigger($trigger)

];
executionConditions.setAdditionalData(additionalData)



request_body.setExecutionConditions($executionConditions)
tasksTask1 = Task()
tasksTask1.setCategory(LifecycleTaskCategory('leaver'))

tasksTask1.setContinueOnError(false)

tasksTask1.setDescription('Remove all licenses assigned to the user')

tasksTask1.setDisplayName('Remove all licenses for user')

tasksTask1.setExecutionSequence(1)

tasksTask1.setIsEnabled(true)

tasksTask1.setTaskDefinitionId('8fa97d28-3e52-4985-b3a9-a1126f9b8b4e')

tasksTask1.setArguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.setCategory(LifecycleTaskCategory('leaver'))

tasksTask2.setContinueOnError(false)

tasksTask2.setDescription('Remove user from all Teams memberships')

tasksTask2.setDisplayName('Remove user from all Teams')

tasksTask2.setExecutionSequence(2)

tasksTask2.setIsEnabled(true)

tasksTask2.setTaskDefinitionId('81f7b200-2816-4b3b-8c5d-dc556f07b024')

tasksTask2.setArguments([])


tasksArray []= tasksTask2;
tasksTask3 = Task()
tasksTask3.setCategory(LifecycleTaskCategory('leaver'))

tasksTask3.setContinueOnError(false)

tasksTask3.setDescription('Delete user account in Azure AD')

tasksTask3.setDisplayName('Delete User Account')

tasksTask3.setExecutionSequence(3)

tasksTask3.setIsEnabled(true)

tasksTask3.setTaskDefinitionId('8d18588d-9ad3-4c0f-99d0-ec215f0e3dff')

tasksTask3.setArguments([])


tasksArray []= tasksTask3;
request_body.setTasks(tasksArray)




result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body, headers=)


```
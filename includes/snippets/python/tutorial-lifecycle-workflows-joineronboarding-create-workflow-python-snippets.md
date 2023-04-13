---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.displayName = 'Onboard pre-hire employee'

request_body.description = 'Configure pre-hire tasks for onboarding employees before their first day'

request_body.is_enabled = True

request_body.is_scheduling_enabled = False

execution_conditions = WorkflowExecutionConditions()
executionConditions.@odatatype = 'microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => execution_conditions = Scope()
		executionConditions.@odatatype = 'microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		executionConditions.rule = '(department eq \'Sales\')'


executionConditions.scope = scope

'trigger' => execution_conditions = Trigger()
		executionConditions.@odatatype = 'microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		executionConditions.timeBasedAttribute = 'employeeHireDate'

		executionConditions.offset_in_days = -2


executionConditions.trigger = trigger

];
executionConditions.additionaldata(additionalData)



request_body.execution_conditions = executionConditions
tasks_task1 = Task()
tasksTask1.is_enabled = True

tasksTask1.Category(LifecycleTaskCategory('joiner'))

tasksTask1.taskDefinitionId = '1b555e50-7f65-41d5-b514-5894a026d10d'

tasksTask1.displayName = 'Generate TAP And Send Email'

tasksTask1.description = 'Generate Temporary Access Pass and send via email to user\'s manager'

arguments_key_value_pair1 = KeyValuePair()
argumentsKeyValuePair1.name = 'tapLifetimeMinutes'

argumentsKeyValuePair1.value = '480'


argumentsArray []= argumentsKeyValuePair1;
arguments_key_value_pair2 = KeyValuePair()
argumentsKeyValuePair2.name = 'tapIsUsableOnce'

argumentsKeyValuePair2.value = 'true'


argumentsArray []= argumentsKeyValuePair2;
tasksTask1.arguments(argumentsArray)



tasksArray []= tasksTask1;
request_body.tasks(tasksArray)





result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body = request_body)


```
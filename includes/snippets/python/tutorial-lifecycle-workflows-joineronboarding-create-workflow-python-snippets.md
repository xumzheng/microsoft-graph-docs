---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.displayName = 'Onboard pre-hire employee'

request_body.description = 'Configure pre-hire tasks for onboarding employees before their first day'

request_body.isEnabled = true

request_body.isSchedulingEnabled = false

executionConditions = WorkflowExecutionConditions()
executionConditions.@odatatype = 'microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => executionConditions = Scope()
		executionConditions.@odatatype = 'microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		executionConditions.rule = '(department eq \'Sales\')'


executionConditions.scope = scope

'trigger' => executionConditions = Trigger()
		executionConditions.@odatatype = 'microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		executionConditions.timeBasedAttribute = 'employeeHireDate'

		executionConditions.offsetInDays = -2


executionConditions.trigger = trigger

];
executionConditions.additionaldata(additionalData)



request_body.executionConditions = executionConditions
tasksTask1 = Task()
tasksTask1.isEnabled = true

tasksTask1.Category(LifecycleTaskCategory('joiner'))

tasksTask1.taskDefinitionId = '1b555e50-7f65-41d5-b514-5894a026d10d'

tasksTask1.displayName = 'Generate TAP And Send Email'

tasksTask1.description = 'Generate Temporary Access Pass and send via email to user\'s manager'

argumentsKeyValuePair1 = KeyValuePair()
argumentsKeyValuePair1.name = 'tapLifetimeMinutes'

argumentsKeyValuePair1.value = '480'


argumentsArray []= argumentsKeyValuePair1;
argumentsKeyValuePair2 = KeyValuePair()
argumentsKeyValuePair2.name = 'tapIsUsableOnce'

argumentsKeyValuePair2.value = 'true'


argumentsArray []= argumentsKeyValuePair2;
tasksTask1.arguments(argumentsArray)



tasksArray []= tasksTask1;
request_body.tasks(tasksArray)





result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body = request_body)


```
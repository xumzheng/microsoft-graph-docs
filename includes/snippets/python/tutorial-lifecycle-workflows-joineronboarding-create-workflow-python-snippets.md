---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Workflow()
request_body.setDisplayName('Onboard pre-hire employee')

request_body.setDescription('Configure pre-hire tasks for onboarding employees before their first day')

request_body.setIsEnabled(true)

request_body.setIsSchedulingEnabled(false)

executionConditions = WorkflowExecutionConditions()
executionConditions.set@odatatype('microsoft.graph.identityGovernance.triggerAndScopeBasedConditions')

additionalData = [
'scope' => executionConditions = Scope()
		executionConditions.set@odatatype('microsoft.graph.identityGovernance.ruleBasedSubjectSet')

		executionConditions.setRule('(department eq \'Sales\')')


executionConditions.setScope($scope)

'trigger' => executionConditions = Trigger()
		executionConditions.set@odatatype('microsoft.graph.identityGovernance.timeBasedAttributeTrigger')

		executionConditions.setTimeBasedAttribute('employeeHireDate')

		executionConditions.setOffsetInDays(-2)


executionConditions.setTrigger($trigger)

];
executionConditions.setAdditionalData(additionalData)



request_body.setExecutionConditions($executionConditions)
tasksTask1 = Task()
tasksTask1.setIsEnabled(true)

tasksTask1.setCategory(LifecycleTaskCategory('joiner'))

tasksTask1.setTaskDefinitionId('1b555e50-7f65-41d5-b514-5894a026d10d')

tasksTask1.setDisplayName('Generate TAP And Send Email')

tasksTask1.setDescription('Generate Temporary Access Pass and send via email to user\'s manager')

argumentsKeyValuePair1 = KeyValuePair()
argumentsKeyValuePair1.setName('tapLifetimeMinutes')

argumentsKeyValuePair1.setValue('480')


argumentsArray []= argumentsKeyValuePair1;
argumentsKeyValuePair2 = KeyValuePair()
argumentsKeyValuePair2.setName('tapIsUsableOnce')

argumentsKeyValuePair2.setValue('true')


argumentsArray []= argumentsKeyValuePair2;
tasksTask1.setArguments(argumentsArray)



tasksArray []= tasksTask1;
request_body.setTasks(tasksArray)




result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Workflow()
request_body.Category(LifecycleWorkflowCategory('joiner'))

request_body.description = 'Configure new hire tasks for onboarding employees on their first day'

request_body.displayName = 'Australia Onboard new hire employee'

request_body.isEnabled = true

request_body.isSchedulingEnabled = false

executionConditions = WorkflowExecutionConditions()
executionConditions.@odatatype = '#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => executionConditions = Scope()
		executionConditions.@odatatype = '#microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		executionConditions.rule = '(country eq \'Australia\')'


executionConditions.scope = scope

'trigger' => executionConditions = Trigger()
		executionConditions.@odatatype = '#microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		executionConditions.timeBasedAttribute = 'employeeHireDate'

		executionConditions.offsetInDays = 0


executionConditions.trigger = trigger

];
executionConditions.additionaldata(additionalData)



request_body.executionConditions = executionConditions
tasksTask1 = Task()
tasksTask1.continueOnError = false

tasksTask1.description = 'Enable user account in the directory'

tasksTask1.displayName = 'Enable User Account'

tasksTask1.isEnabled = true

tasksTask1.taskDefinitionId = '6fc52c9d-398b-4305-9763-15f42c1676fc'

tasksTask1.Arguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.continueOnError = false

tasksTask2.description = 'Send welcome email to new hire'

tasksTask2.displayName = 'Send Welcome Email'

tasksTask2.isEnabled = true

tasksTask2.taskDefinitionId = '70b29d51-b59a-4773-9280-8841dfd3f2ea'

tasksTask2.Arguments([])


tasksArray []= tasksTask2;
request_body.tasks(tasksArray)





result = await client.identityGovernance.lifecycleWorkflows.workflows.post(request_body = request_body)


```
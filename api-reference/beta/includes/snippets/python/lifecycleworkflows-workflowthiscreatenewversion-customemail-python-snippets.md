---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateNewVersionPostRequestBody()
workflow = Workflow()
workflow.Category(LifecycleWorkflowCategory('joiner'))

workflow.description = 'Configure new hire tasks for onboarding employees on their first day'

workflow.displayName = 'Global onboard new hire employee'

workflow.isEnabled = true

workflow.isSchedulingEnabled = false

workflowExecutionConditions = WorkflowExecutionConditions()
workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => workflowExecutionConditions = Scope()
		workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		workflowExecutionConditions.rule = '(department eq \'Marketing\')'


workflowExecutionConditions.scope = scope

'trigger' => workflowExecutionConditions = Trigger()
		workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		workflowExecutionConditions.timeBasedAttribute = 'employeeHireDate'

		workflowExecutionConditions.offsetInDays = 1


workflowExecutionConditions.trigger = trigger

];
workflowExecutionConditions.additionaldata(additionalData)



workflow.executionConditions = workflowExecutionConditions
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

argumentsKeyValuePair1 = KeyValuePair()
argumentsKeyValuePair1.name = 'cc'

argumentsKeyValuePair1.value = '1baa57fa-3c4e-4526-ba5a-db47a9df95f0'


argumentsArray []= argumentsKeyValuePair1;
argumentsKeyValuePair2 = KeyValuePair()
argumentsKeyValuePair2.name = 'customSubject'

argumentsKeyValuePair2.value = 'Welcome to the organization {{userDisplayName}}!'


argumentsArray []= argumentsKeyValuePair2;
argumentsKeyValuePair3 = KeyValuePair()
argumentsKeyValuePair3.name = 'customBody'

argumentsKeyValuePair3.value = 'Welcome to our organization {{userGivenName}}!'


argumentsArray []= argumentsKeyValuePair3;
argumentsKeyValuePair4 = KeyValuePair()
argumentsKeyValuePair4.name = 'locale'

argumentsKeyValuePair4.value = 'en-us'


argumentsArray []= argumentsKeyValuePair4;
tasksTask2.arguments(argumentsArray)



tasksArray []= tasksTask2;
workflow.tasks(tasksArray)



request_body.workflow = workflow



result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').identityGovernancecreateNewVersion.post(request_body = request_body)


```
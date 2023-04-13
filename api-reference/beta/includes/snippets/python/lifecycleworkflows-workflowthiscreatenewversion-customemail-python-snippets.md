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

workflow.is_enabled = True

workflow.is_scheduling_enabled = False

workflow_execution_conditions = WorkflowExecutionConditions()
workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions'

additionalData = [
'scope' => workflow_execution_conditions = Scope()
		workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.ruleBasedSubjectSet'

		workflowExecutionConditions.rule = '(department eq \'Marketing\')'


workflowExecutionConditions.scope = scope

'trigger' => workflow_execution_conditions = Trigger()
		workflowExecutionConditions.@odatatype = '#microsoft.graph.identityGovernance.timeBasedAttributeTrigger'

		workflowExecutionConditions.timeBasedAttribute = 'employeeHireDate'

		workflowExecutionConditions.offset_in_days = 1


workflowExecutionConditions.trigger = trigger

];
workflowExecutionConditions.additionaldata(additionalData)



workflow.execution_conditions = workflowExecutionConditions
tasks_task1 = Task()
tasksTask1.continue_on_error = False

tasksTask1.description = 'Enable user account in the directory'

tasksTask1.displayName = 'Enable User Account'

tasksTask1.is_enabled = True

tasksTask1.taskDefinitionId = '6fc52c9d-398b-4305-9763-15f42c1676fc'

tasksTask1.Arguments([])


tasksArray []= tasksTask1;
tasks_task2 = Task()
tasksTask2.continue_on_error = False

tasksTask2.description = 'Send welcome email to new hire'

tasksTask2.displayName = 'Send Welcome Email'

tasksTask2.is_enabled = True

tasksTask2.taskDefinitionId = '70b29d51-b59a-4773-9280-8841dfd3f2ea'

arguments_key_value_pair1 = KeyValuePair()
argumentsKeyValuePair1.name = 'cc'

argumentsKeyValuePair1.value = '1baa57fa-3c4e-4526-ba5a-db47a9df95f0'


argumentsArray []= argumentsKeyValuePair1;
arguments_key_value_pair2 = KeyValuePair()
argumentsKeyValuePair2.name = 'customSubject'

argumentsKeyValuePair2.value = 'Welcome to the organization {{userDisplayName}}!'


argumentsArray []= argumentsKeyValuePair2;
arguments_key_value_pair3 = KeyValuePair()
argumentsKeyValuePair3.name = 'customBody'

argumentsKeyValuePair3.value = 'Welcome to our organization {{userGivenName}}!'


argumentsArray []= argumentsKeyValuePair3;
arguments_key_value_pair4 = KeyValuePair()
argumentsKeyValuePair4.name = 'locale'

argumentsKeyValuePair4.value = 'en-us'


argumentsArray []= argumentsKeyValuePair4;
tasksTask2.arguments(argumentsArray)



tasksArray []= tasksTask2;
workflow.tasks(tasksArray)



request_body.workflow = workflow



result = await client.identityGovernance.lifecycleWorkflows.workflows_by_id('workflow-id').identityGovernancecreateNewVersion.post(request_body = request_body)


```
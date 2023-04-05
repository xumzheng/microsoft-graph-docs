---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreateNewVersionPostRequestBody()
workflow = Workflow()
workflow.setCategory(LifecycleWorkflowCategory('joiner'))

workflow.setDescription('Configure new hire tasks for onboarding employees on their first day')

workflow.setDisplayName('Global onboard new hire employee')

workflow.setIsEnabled(true)

workflow.setIsSchedulingEnabled(false)

workflowExecutionConditions = WorkflowExecutionConditions()
workflowExecutionConditions.set@odatatype('#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions')

additionalData = [
'scope' => workflowExecutionConditions = Scope()
		workflowExecutionConditions.set@odatatype('#microsoft.graph.identityGovernance.ruleBasedSubjectSet')

		workflowExecutionConditions.setRule('(department eq \'Marketing\')')


workflowExecutionConditions.setScope($scope)

'trigger' => workflowExecutionConditions = Trigger()
		workflowExecutionConditions.set@odatatype('#microsoft.graph.identityGovernance.timeBasedAttributeTrigger')

		workflowExecutionConditions.setTimeBasedAttribute('employeeHireDate')

		workflowExecutionConditions.setOffsetInDays(1)


workflowExecutionConditions.setTrigger($trigger)

];
workflowExecutionConditions.setAdditionalData(additionalData)



workflow.setExecutionConditions($workflowExecutionConditions)
tasksTask1 = Task()
tasksTask1.setContinueOnError(false)

tasksTask1.setDescription('Enable user account in the directory')

tasksTask1.setDisplayName('Enable User Account')

tasksTask1.setIsEnabled(true)

tasksTask1.setTaskDefinitionId('6fc52c9d-398b-4305-9763-15f42c1676fc')

tasksTask1.setArguments([])


tasksArray []= tasksTask1;
tasksTask2 = Task()
tasksTask2.setContinueOnError(false)

tasksTask2.setDescription('Send welcome email to new hire')

tasksTask2.setDisplayName('Send Welcome Email')

tasksTask2.setIsEnabled(true)

tasksTask2.setTaskDefinitionId('70b29d51-b59a-4773-9280-8841dfd3f2ea')

tasksTask2.setArguments([])


tasksArray []= tasksTask2;
workflow.setTasks(tasksArray)



request_body.setWorkflow($workflow)


result = await client.identityGovernance.lifecycleWorkflows.workflowsById('workflow-id').identityGovernancecreateNewVersion.post(request_body)


```
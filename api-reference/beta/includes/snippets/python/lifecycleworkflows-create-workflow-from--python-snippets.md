---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Workflow();
requestBody.setCategory(LifecycleWorkflowCategory('joiner'));

requestBody.setDescription('Configure new hire tasks for onboarding employees on their first day');

requestBody.setDisplayName('Australia Onboard new hire employee');

requestBody.setIsEnabled(true);

requestBody.setIsSchedulingEnabled(false);

executionConditions = WorkflowExecutionConditions();
executionConditions.set@odatatype('#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions');

additionalData = [
'scope' => executionConditions = Scope();
		executionConditions.set@odatatype('#microsoft.graph.identityGovernance.ruleBasedSubjectSet');

		executionConditions.setRule('(country eq \'Australia\')');


executionConditions.setScope($scope);

'trigger' => executionConditions = Trigger();
		executionConditions.set@odatatype('#microsoft.graph.identityGovernance.timeBasedAttributeTrigger');

		executionConditions.setTimeBasedAttribute('employeeHireDate');

		executionConditions.setOffsetInDays(0);


executionConditions.setTrigger($trigger);

];
executionConditions.setAdditionalData(additionalData);



requestBody.setExecutionConditions($executionConditions);
tasksTask1 = Task();
tasksTask1.setContinueOnError(false);

tasksTask1.setDescription('Enable user account in the directory');

tasksTask1.setDisplayName('Enable User Account');

tasksTask1.setIsEnabled(true);

tasksTask1.setTaskDefinitionId('6fc52c9d-398b-4305-9763-15f42c1676fc');

tasksTask1.setArguments([]);


tasksArray []= tasksTask1;
tasksTask2 = Task();
tasksTask2.setContinueOnError(false);

tasksTask2.setDescription('Send welcome email to new hire');

tasksTask2.setDisplayName('Send Welcome Email');

tasksTask2.setIsEnabled(true);

tasksTask2.setTaskDefinitionId('70b29d51-b59a-4773-9280-8841dfd3f2ea');

tasksTask2.setArguments([]);


tasksArray []= tasksTask2;
requestBody.setTasks(tasksArray);




result = await client.identityGovernance().lifecycleWorkflows().workflows().post(requestBody);


```
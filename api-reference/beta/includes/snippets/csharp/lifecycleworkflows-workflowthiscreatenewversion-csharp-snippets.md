---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreateNewVersionPostRequestBody
{
	Workflow = new Workflow
	{
		Description = "Configure new hire tasks for onboarding employees on their first day",
		DisplayName = "Global onboard new hire employee",
		IsEnabled = true,
		IsSchedulingEnabled = false,
		ExecutionConditions = new WorkflowExecutionConditions
		{
			OdataType = "#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions",
			AdditionalData = new Dictionary<string, object>
			{
				{
					"scope" , new 
					{
						OdataType = "#microsoft.graph.identityGovernance.ruleBasedSubjectSet",
						Rule = "(department eq 'Marketing')",
					}
				},
				{
					"trigger" , new 
					{
						OdataType = "#microsoft.graph.identityGovernance.timeBasedAttributeTrigger",
						TimeBasedAttribute = "employeeHireDate",
						OffsetInDays = 1,
					}
				},
			},
		},
		Tasks = new List<Task>
		{
			new Task
			{
				ContinueOnError = false,
				Description = "Enable user account in the directory",
				DisplayName = "Enable User Account",
				IsEnabled = true,
				TaskDefinitionId = "6fc52c9d-398b-4305-9763-15f42c1676fc",
				Arguments = new List<>
				{
				},
			},
			new Task
			{
				ContinueOnError = false,
				Description = "Send welcome email to new hire",
				DisplayName = "Send Welcome Email",
				IsEnabled = true,
				TaskDefinitionId = "70b29d51-b59a-4773-9280-8841dfd3f2ea",
				Arguments = new List<>
				{
				},
			},
		},
	},
};
var result = await graphClient.IdentityGovernance.LifecycleWorkflows.Workflows["workflow-id"].CreateNewVersion.PostAsync(requestBody);


```
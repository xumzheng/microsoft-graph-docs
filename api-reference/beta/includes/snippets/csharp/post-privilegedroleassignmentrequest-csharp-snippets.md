---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrivilegedRoleAssignmentRequest
{
	Duration = "2",
	Reason = "Activate the role for business purpose",
	TicketNumber = "234",
	TicketSystem = "system",
	Schedule = new GovernanceSchedule
	{
		StartDateTime = DateTimeOffset.Parse("2018-02-08T02:35:17.903Z"),
	},
	Type = "UserAdd",
	AssignmentState = "Active",
	RoleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
};
var result = await graphClient.PrivilegedRoleAssignmentRequests.PostAsync(requestBody);


```
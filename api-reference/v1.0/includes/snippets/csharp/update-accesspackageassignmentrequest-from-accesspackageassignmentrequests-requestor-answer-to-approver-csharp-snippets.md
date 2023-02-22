---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentRequest = new AccessPackageAssignmentRequestObject
{
	Id = "7a6ab703-0780-4b37-8445-81f679b2d75c",
	RequestType = AccessPackageRequestType.AdminUpdate,
	Answers = new List<AccessPackageAnswer>()
	{
		new AccessPackageAnswerString
		{
			Value = "UpdatedAnswerValue",
			AnsweredQuestion = new AccessPackageMultipleChoiceQuestion
			{
				Id = "8fe745e7-80b2-490d-bd22-4e708c77288c"
			}
		},
		new AccessPackageAnswerString
		{
			Value = "My updated answer.",
			DisplayValue = "This is my updated answer to the question.",
			AnsweredQuestion = new AccessPackageTextInputQuestion
			{
				Id = "7aaa18c9-8e4f-440f-bd5a-3a7ce312cbe6"
			}
		}
	},
	Assignment = new AccessPackageAssignment
	{
		Id = "44c741c1-2cf4-40db-83b6-e0112f8e5a83"
	}
};

await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests
	.Request()
	.AddAsync(accessPackageAssignmentRequest);

```
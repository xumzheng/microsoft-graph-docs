---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationSchool
{
	@odata.type = "#microsoft.graph.educationSchool",
	DisplayName = "String",
	Description = "String",
	ExternalSource = "String",
	ExternalSourceDetail = "String",
	PrincipalEmail = "String",
	PrincipalName = "String",
	ExternalPrincipalId = "String",
	LowestGrade = "String",
	HighestGrade = "String",
	SchoolNumber = "String",
	ExternalId = "String",
	Phone = "String",
	Fax = "String",
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
	Address = new PhysicalAddress
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.physicalAddress"},
		}
	},
};
var result = await graphClient.Education.Schools.PostAsync(requestBody);


```
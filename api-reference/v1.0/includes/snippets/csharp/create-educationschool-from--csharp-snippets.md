---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationSchool
{
	OdataType = "#microsoft.graph.educationSchool",
	DisplayName = "String",
	Description = "String",
	ExternalSource = EducationExternalSource.String,
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
		OdataType = "microsoft.graph.identitySet",
	},
	Address = new PhysicalAddress
	{
		OdataType = "microsoft.graph.physicalAddress",
	},
};
var result = await graphClient.Education.Schools.PostAsync(requestBody);


```
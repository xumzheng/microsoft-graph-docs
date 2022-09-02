---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationClass
{
	OdataType = "#microsoft.graph.educationClass",
	DisplayName = "String",
	MailNickname = "String",
	Description = "String",
	CreatedBy = new IdentitySet
	{
		OdataType = "microsoft.graph.identitySet",
	},
	ClassCode = "String",
	ExternalName = "String",
	ExternalId = "String",
	ExternalSource = EducationExternalSource.String,
	ExternalSourceDetail = "String",
	Grade = "String",
	Term = new EducationTerm
	{
		OdataType = "microsoft.graph.educationTerm",
	},
};
var result = await graphClient.Education.Classes.PostAsync(requestBody);


```
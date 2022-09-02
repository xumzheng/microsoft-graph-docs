---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SubjectRightsRequest
{
	Type = SubjectRightsRequestType.SubjectRightsRequestType,
	DataSubjectType = DataSubjectType.DataSubjectType,
	Regulations = new List<string>
	{
		"String",
	},
	DisplayName = "String",
	Description = "String",
	InternalDueDateTime = DateTimeOffset.Parse("String (timestamp)"),
	DataSubject = new DataSubject
	{
		FirstName = "String",
		LastName = "String",
		Email = "String",
		Residency = "String",
		AdditionalData = new Dictionary<string, object>
		{
			{
				"phoneNumber" , "String"
			},
			{
				"SSN" , "String"
			},
		},
	},
};
var result = await graphClient.Privacy.SubjectRightsRequests.PostAsync(requestBody);


```
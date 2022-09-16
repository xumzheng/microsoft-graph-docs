---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationalActivity
{
	CompletionMonthYear = "Date",
	EndMonthYear = "Date",
	Institution = new InstitutionData
	{
		Description = null,
		DisplayName = "Colorado State University",
		Location = new PhysicalAddress
		{
			Type = PhysicalAddressType.Business,
			PostOfficeBox = null,
			Street = "12000 E Prospect Rd",
			City = "Fort Collins",
			State = "Colorado",
			CountryOrRegion = "USA",
			PostalCode = "80525",
		},
		WebUrl = "https://www.colostate.edu",
	},
	Program = new EducationalActivityDetail
	{
		Abbreviation = "MBA",
		Activities = null,
		Awards = null,
		Description = "Master of Business Administration with a major in Entreprenuership and Finance.",
		DisplayName = "Master of Business Administration",
		FieldsOfStudy = null,
		Grade = "3.9",
		Notes = null,
		WebUrl = "https://biz.colostate.edu",
	},
	StartMonthYear = "Date",
};
var result = await graphClient.Me.Profile.EducationalActivities.PostAsync(requestBody);


```
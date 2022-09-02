---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationUser
{
	OdataType = "#microsoft.graph.educationUser",
	PrimaryRole = EducationUserRole.String,
	MiddleName = "String",
	ExternalSource = EducationExternalSource.String,
	ExternalSourceDetail = "String",
	ResidenceAddress = new PhysicalAddress
	{
		OdataType = "microsoft.graph.physicalAddress",
	},
	MailingAddress = new PhysicalAddress
	{
		OdataType = "microsoft.graph.physicalAddress",
	},
	Student = new EducationStudent
	{
		OdataType = "microsoft.graph.educationStudent",
	},
	Teacher = new EducationTeacher
	{
		OdataType = "microsoft.graph.educationTeacher",
	},
	CreatedBy = new IdentitySet
	{
		OdataType = "microsoft.graph.identitySet",
	},
	AccountEnabled = boolean,
	AssignedLicenses = new List<AssignedLicense>
	{
		new AssignedLicense
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "microsoft.graph.assignedLicense"
				},
			},
		},
	},
	AssignedPlans = new List<AssignedPlan>
	{
		new AssignedPlan
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "microsoft.graph.assignedPlan"
				},
			},
		},
	},
	BusinessPhones = new List<>
	{
		"String",
	},
	Department = "String",
	DisplayName = "String",
	GivenName = "String",
	Mail = "String",
	MailNickname = "String",
	MobilePhone = "String",
	PasswordPolicies = "String",
	PasswordProfile = new PasswordProfile
	{
		OdataType = "microsoft.graph.passwordProfile",
	},
	OfficeLocation = "String",
	PreferredLanguage = "String",
	ProvisionedPlans = new List<ProvisionedPlan>
	{
		new ProvisionedPlan
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"@odata.type" , "microsoft.graph.provisionedPlan"
				},
			},
		},
	},
	RefreshTokensValidFromDateTime = DateTimeOffset.Parse("String (timestamp)"),
	ShowInAddressList = boolean,
	Surname = "String",
	UsageLocation = "String",
	UserPrincipalName = "String",
	UserType = "String",
	OnPremisesInfo = new EducationOnPremisesInfo
	{
		OdataType = "microsoft.graph.educationOnPremisesInfo",
	},
};
var result = await graphClient.Education.Users.PostAsync(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationUser
{
	@odata.type = "#microsoft.graph.educationUser",
	PrimaryRole = "String",
	MiddleName = "String",
	ExternalSource = "String",
	ExternalSourceDetail = "String",
	ResidenceAddress = new PhysicalAddress
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.physicalAddress"},
		}
	},
	MailingAddress = new PhysicalAddress
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.physicalAddress"},
		}
	},
	Student = new EducationStudent
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.educationStudent"},
		}
	},
	Teacher = new EducationTeacher
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.educationTeacher"},
		}
	},
	CreatedBy = new IdentitySet
	{
		@odata.type = "microsoft.graph.identitySet",
	},
	AccountEnabled = "Boolean",
	AssignedLicenses = new List<AssignedLicense>
	{
		new AssignedLicense
		{
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.assignedLicense"},
			}
		},
	}
	AssignedPlans = new List<AssignedPlan>
	{
		new AssignedPlan
		{
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.assignedPlan"},
			}
		},
	}
	BusinessPhones = new List<String>
	{
		"String",
	}
	Department = "String",
	DisplayName = "String",
	GivenName = "String",
	Mail = "String",
	MailNickname = "String",
	MobilePhone = "String",
	PasswordPolicies = "String",
	PasswordProfile = new PasswordProfile
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.passwordProfile"},
		}
	},
	OfficeLocation = "String",
	PreferredLanguage = "String",
	ProvisionedPlans = new List<ProvisionedPlan>
	{
		new ProvisionedPlan
		{
			AdditionalData = new()
			{
				{"@odata.type", "microsoft.graph.provisionedPlan"},
			}
		},
	}
	RefreshTokensValidFromDateTime = DateTimeOffset.Parse("String (timestamp)"),
	ShowInAddressList = "Boolean",
	Surname = "String",
	UsageLocation = "String",
	UserPrincipalName = "String",
	UserType = "String",
	OnPremisesInfo = new EducationOnPremisesInfo
	{
		AdditionalData = new()
		{
			{"@odata.type", "microsoft.graph.educationOnPremisesInfo"},
		}
	},
};
var result = await graphClient.Education.Users.PostAsync(requestBody);


```
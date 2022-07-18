---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EvaluateApplicationRequestBody
{
	ContentInfo = new ContentInfo
	{
		Format = "default",
		Identifier = null,
		State = "rest",
		Metadata = new List<KeyValuePair>
		{
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
				Value = "True",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
				Value = "Standard",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
				Value = "1/1/0001 12:00:00 AM",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
				Value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
				Value = "General",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
				Value = "0",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
			new KeyValuePair
			{
				Name = "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
				Value = "00000000-0000-0000-0000-000000000000",
				AdditionalData = new()
				{
					{"@odata.type", "#microsoft.graph.keyValuePair"},
				}
			},
		}
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.contentInfo"},
			{"format@odata.type", "#microsoft.graph.contentFormat"},
			{"state@odata.type", "#microsoft.graph.contentState"},
			{"metadata@odata.type", "#Collection(microsoft.graph.keyValuePair)"},
		}
	},
	LabelingOptions = new LabelingOptions
	{
		AssignmentMethod = "standard",
		LabelId = "97309856-9c28-4ac6-9382-5f8bc20c457b",
		DowngradeJustification = null,
		ExtendedProperties = new List<KeyValuePair>
		{
		}
		AdditionalData = new()
		{
			{"@odata.type", "#microsoft.graph.labelingOptions"},
			{"assignmentMethod@odata.type", "#microsoft.graph.assignmentMethod"},
			{"labelId@odata.type", "#Guid"},
			{"extendedProperties@odata.type", "#Collection(microsoft.graph.keyValuePair)"},
		}
	},
};
var result = await graphClient.InformationProtection.Policy.Labels.EvaluateApplication.PostAsync(requestBody, (requestConfiguration) =>
{
	requestConfiguration.Headers.Add("User-Agent", "ContosoLOBApp/1.0");
});


```
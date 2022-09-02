---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchemaExtension
{
	Id = "courses",
	Description = "Graph Learn training courses extensions",
	TargetTypes = new List<>
	{
		"Group",
	},
	Properties = new List<ExtensionSchemaProperty>
	{
		new ExtensionSchemaProperty
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"name" , "courseId"
				},
				{
					"type" , "Integer"
				},
			},
		},
		new ExtensionSchemaProperty
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"name" , "courseName"
				},
				{
					"type" , "String"
				},
			},
		},
		new ExtensionSchemaProperty
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"name" , "courseType"
				},
				{
					"type" , "String"
				},
			},
		},
	},
};
var result = await graphClient.SchemaExtensions.PostAsync(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new SchemaExtension
{
	Owner = "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa",
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
		new ExtensionSchemaProperty
		{
			AdditionalData = new Dictionary<string, object>
			{
				{
					"name" , "courseSupervisors"
				},
				{
					"type" , "String"
				},
			},
		},
	},
};
await graphClient.SchemaExtensions["schemaExtension-id"].PatchAsync(requestBody);


```
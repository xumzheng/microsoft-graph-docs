---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ColumnDefinition
{
	Description = "test",
	EnforceUniqueValues = false,
	Hidden = false,
	Indexed = false,
	Name = "Title",
	Text = new TextColumn
	{
		AllowMultipleLines = false,
		AppendChangesToExistingText = false,
		LinesForEditing = 0,
		MaxLength = 255,
	},
};
var result = await graphClient.Sites["site-id"].Lists["list-id"].Columns.PostAsync(requestBody);


```
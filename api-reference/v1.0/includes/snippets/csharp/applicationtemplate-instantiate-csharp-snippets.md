---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new InstantiatePostRequestBody
{
	DisplayName = "Azure AD SAML Toolkit",
};
var result = await graphClient.ApplicationTemplates["applicationTemplate-id"].Instantiate.PostAsync(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OAuth2PermissionGrant
{
	Scope = "User.ReadBasic.All Group.ReadWrite.All",
};
var result = await graphClient.Oauth2PermissionGrants["oAuth2PermissionGrant-id"].PatchAsync(requestBody);


```
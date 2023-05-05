---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-sdk-go/drives"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestParameters := &graphconfig.DriveItemRootRequestBuilderGetQueryParameters{
	Expand: [] string {"children"},
}
configuration := &graphconfig.DriveItemRootRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Drives().ByDriveId("drive-id").Root().Get(context.Background(), configuration)


```
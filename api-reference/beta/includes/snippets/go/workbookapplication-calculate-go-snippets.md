---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Drives/Item/Items/Item/Workbook/Application/Calculate"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewCalculatePostRequestBody()
calculationType := "calculationType-value"
requestBody.SetCalculationType(&calculationType) 

graphClient.Drives().ByDriveId("drive-id").Items().ByItemId("driveItem-id").Workbook().Application().Calculate().Post(context.Background(), requestBody, nil)


```
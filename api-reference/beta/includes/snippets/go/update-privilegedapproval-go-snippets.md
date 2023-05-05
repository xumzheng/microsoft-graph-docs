---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewPrivilegedApproval()
approvalState := graphmodels.APPROVALSTATE-VALUE_APPROVALSTATE 
requestBody.SetApprovalState(&approvalState) 
approverReason := "approverReason-value"
requestBody.SetApproverReason(&approverReason) 

result, err := graphClient.PrivilegedApproval().ByPrivilegedApproval().Id("privilegedApproval-id").Patch(context.Background(), requestBody, nil)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models//identityGovernance"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewLifecycleManagementSettings()
workflowScheduleIntervalInHours := int32(3)
requestBody.SetWorkflowScheduleIntervalInHours(&workflowScheduleIntervalInHours) 
additionalData := map[string]interface{}{
	"odataContext" : "https://graph.microsoft.com/beta/$metadata#identityGovernance/lifecycleWorkflows/settings/$entity", 
emailSettings := graphmodels.New()
senderDomain := "ContosoIndustries.net"
emailSettings.SetSenderDomain(&senderDomain) 
	useCompanyBranding := true
emailSettings.SetUseCompanyBranding(&useCompanyBranding) 
	requestBody.SetEmailSettings(emailSettings)
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.IdentityGovernance().LifecycleWorkflows().Settings().Patch(context.Background(), requestBody, nil)


```
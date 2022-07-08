---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewUpdateAlertsPostRequestBody()


alert := graphmodels.NewAlert()
additionalData := map[string]interface{}{
	"assignedTo" : "String", 
	"closedDateTime" : "String (timestamp)", 
	comments := []String {
		"String",

	}
feedback := graphmodels.New()
"@odata.type" := "microsoft.graph.alertFeedback"
feedback.Set"@odata.type"(&"@odata.type") 
	alert.SetFeedback(feedback)
	"id" : "String (identifier)", 
status := graphmodels.New()
"@odata.type" := "microsoft.graph.alertStatus"
status.Set"@odata.type"(&"@odata.type") 
	alert.SetStatus(status)
	tags := []String {
		"String",

	}
vendorInformation := graphmodels.New()
provider := "String"
vendorInformation.SetProvider(&provider) 
vendor := "String"
vendorInformation.SetVendor(&vendor) 
	alert.SetVendorInformation(vendorInformation)
}
alert.SetAdditionalData(additionalData)

value := []graphmodels.Alertable {
	alert,

}
requestBody.SetValue(value)

result, err := graphClient.Security().Alerts().UpdateAlerts().Post(requestBody)


```
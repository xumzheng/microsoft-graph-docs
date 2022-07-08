---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := graphmodels.NewAssignPostRequestBody()


cloudPcUserSettingAssignment := graphmodels.NewCloudPcUserSettingAssignment()
additionalData := map[string]interface{}{
	"id" : "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff", 
target := graphmodels.New()
"@odata.type" := "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
target.Set"@odata.type"(&"@odata.type") 
groupId := "64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
target.SetGroupId(&groupId) 
	cloudPcUserSettingAssignment.SetTarget(target)
}
cloudPcUserSettingAssignment.SetAdditionalData(additionalData)

assignments := []graphmodels.CloudPcUserSettingAssignmentable {
	cloudPcUserSettingAssignment,

}
requestBody.SetAssignments(assignments)

graphClient.DeviceManagement().VirtualEndpoint().UserSettingsById("cloudPcUserSetting-id").Assign(cloudPcUserSetting-id).Post(requestBody)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'extension-policy'

request_body.description = 'test'

request_body.accessPackageId = 'ba5807c7-2aa9-4c8a-907e-4a17ee587500'

request_body.canExtend = false

request_body.requestApprovalSettings=null

requestorSettings = RequestorSettings()
requestorSettings.acceptRequests = true

requestorSettings.scopeType = 'AllExistingDirectorySubjects'

requestorSettings.AllowedRequestors([])

additionalData = [
'isOnBehalfAllowed' => false,
];
requestorSettings.additionaldata(additionalData)



request_body.requestorSettings = requestorSettings
request_body.accessReviewSettings=null

request_body.Questions([])

customExtensionStageSettingsCustomExtensionStageSetting1 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting1.Stage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionStageSettingsCustomExtensionStageSetting1.customExtension = customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting1;
customExtensionStageSettingsCustomExtensionStageSetting2 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting2.Stage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionStageSettingsCustomExtensionStageSetting2.customExtension = customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting2;
request_body.customextensionstagesettings(customExtensionStageSettingsArray)


additionalData = [
'expiration' => request_body = Expiration()
request_body.type = 'afterDuration'

request_body.duration = 'P365D'


request_body.expiration = expiration

];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```
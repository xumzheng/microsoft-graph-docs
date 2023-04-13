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

request_body.can_extend = False

request_body.requestApprovalSettings=null

requestor_settings = RequestorSettings()
requestorSettings.accept_requests = True

requestorSettings.scopeType = 'AllExistingDirectorySubjects'

requestorSettings.AllowedRequestors([])

additionalData = [
'isOnBehalfAllowed' => false,
];
requestorSettings.additionaldata(additionalData)



request_body.requestor_settings = requestorSettings
request_body.accessReviewSettings=null

request_body.Questions([])

custom_extension_stage_settings_custom_extension_stage_setting1 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting1.Stage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

custom_extension_stage_settings_custom_extension_stage_setting1_custom_extension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionStageSettingsCustomExtensionStageSetting1.custom_extension = customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting1;
custom_extension_stage_settings_custom_extension_stage_setting2 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting2.Stage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

custom_extension_stage_settings_custom_extension_stage_setting2_custom_extension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionStageSettingsCustomExtensionStageSetting2.custom_extension = customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension

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
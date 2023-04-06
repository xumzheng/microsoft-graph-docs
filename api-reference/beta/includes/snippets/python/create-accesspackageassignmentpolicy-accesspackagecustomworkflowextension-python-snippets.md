---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setDisplayName('extension-policy')

request_body.setDescription('test')

request_body.setAccessPackageId('ba5807c7-2aa9-4c8a-907e-4a17ee587500')

request_body.setCanExtend(false)

request_body.setRequestApprovalSettings(null)

requestorSettings = RequestorSettings()
requestorSettings.setAcceptRequests(true)

requestorSettings.setScopeType('AllExistingDirectorySubjects')

requestorSettings.setAllowedRequestors([])

additionalData = [
'isOnBehalfAllowed' => false,
];
requestorSettings.setAdditionalData(additionalData)



request_body.setRequestorSettings($requestorSettings)
request_body.setAccessReviewSettings(null)

request_body.setQuestions([])

customExtensionStageSettingsCustomExtensionStageSetting1 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting1.setStage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8')


customExtensionStageSettingsCustomExtensionStageSetting1.setCustomExtension($customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension)

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting1;
customExtensionStageSettingsCustomExtensionStageSetting2 = CustomExtensionStageSetting()
customExtensionStageSettingsCustomExtensionStageSetting2.setStage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension = CustomCalloutExtension()
customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8')


customExtensionStageSettingsCustomExtensionStageSetting2.setCustomExtension($customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension)

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting2;
request_body.setCustomExtensionStageSettings(customExtensionStageSettingsArray)


additionalData = [
'expiration' => request_body = Expiration()
request_body.setType('afterDuration')

request_body.setDuration('P365D')


request_body.setExpiration($expiration)

];
request_body.setAdditionalData(additionalData)




result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body, headers=)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessPackageAssignmentPolicy();
requestBody.setDisplayName('extension-policy');

requestBody.setDescription('test');

requestBody.setAccessPackageId('ba5807c7-2aa9-4c8a-907e-4a17ee587500');

requestBody.setCanExtend(false);

requestBody.setRequestApprovalSettings(null);

requestorSettings = RequestorSettings();
requestorSettings.setAcceptRequests(true);

requestorSettings.setScopeType('AllExistingDirectorySubjects');

requestorSettings.setAllowedRequestors([]);

additionalData = [
'isOnBehalfAllowed' => false,
];
requestorSettings.setAdditionalData(additionalData);



requestBody.setRequestorSettings($requestorSettings);
requestBody.setAccessReviewSettings(null);

requestBody.setQuestions([]);

customExtensionStageSettingsCustomExtensionStageSetting1 = CustomExtensionStageSetting();
customExtensionStageSettingsCustomExtensionStageSetting1.setStage(AccessPackageCustomExtensionStage('assignmentrequestcreated'));

customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension = CustomCalloutExtension();
customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8');


customExtensionStageSettingsCustomExtensionStageSetting1.setCustomExtension($customExtensionStageSettingsCustomExtensionStageSetting1CustomExtension);

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting1;
customExtensionStageSettingsCustomExtensionStageSetting2 = CustomExtensionStageSetting();
customExtensionStageSettingsCustomExtensionStageSetting2.setStage(AccessPackageCustomExtensionStage('assignmentrequestgranted'));

customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension = CustomCalloutExtension();
customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8');


customExtensionStageSettingsCustomExtensionStageSetting2.setCustomExtension($customExtensionStageSettingsCustomExtensionStageSetting2CustomExtension);

customExtensionStageSettingsArray []= customExtensionStageSettingsCustomExtensionStageSetting2;
requestBody.setCustomExtensionStageSettings(customExtensionStageSettingsArray);


additionalData = [
'expiration' => requestBody = Expiration();
requestBody.setType('afterDuration');

requestBody.setDuration('P365D');


requestBody.setExpiration($expiration);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies().post(requestBody);


```
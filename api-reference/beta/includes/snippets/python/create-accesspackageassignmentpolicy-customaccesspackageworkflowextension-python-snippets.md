---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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

customExtensionHandlersCustomExtensionHandler1 = CustomExtensionHandler();
customExtensionHandlersCustomExtensionHandler1.setStage(AccessPackageCustomExtensionStage('assignmentrequestcreated'));

customExtensionHandlersCustomExtensionHandler1CustomExtension = CustomAccessPackageWorkflowExtension();
customExtensionHandlersCustomExtensionHandler1CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8');


customExtensionHandlersCustomExtensionHandler1.setCustomExtension($customExtensionHandlersCustomExtensionHandler1CustomExtension);

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler1;
customExtensionHandlersCustomExtensionHandler2 = CustomExtensionHandler();
customExtensionHandlersCustomExtensionHandler2.setStage(AccessPackageCustomExtensionStage('assignmentrequestgranted'));

customExtensionHandlersCustomExtensionHandler2CustomExtension = CustomAccessPackageWorkflowExtension();
customExtensionHandlersCustomExtensionHandler2CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8');


customExtensionHandlersCustomExtensionHandler2.setCustomExtension($customExtensionHandlersCustomExtensionHandler2CustomExtension);

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler2;
requestBody.setCustomExtensionHandlers(customExtensionHandlersArray);


additionalData = [
'expiration' => requestBody = Expiration();
requestBody.setType('afterDuration');

requestBody.setDuration('P365D');


requestBody.setExpiration($expiration);

];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies().post(requestBody);


```
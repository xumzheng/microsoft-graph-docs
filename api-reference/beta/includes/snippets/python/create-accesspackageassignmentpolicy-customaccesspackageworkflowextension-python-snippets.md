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

customExtensionHandlersCustomExtensionHandler1 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler1.setStage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

customExtensionHandlersCustomExtensionHandler1CustomExtension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler1CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8')


customExtensionHandlersCustomExtensionHandler1.setCustomExtension($customExtensionHandlersCustomExtensionHandler1CustomExtension)

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler1;
customExtensionHandlersCustomExtensionHandler2 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler2.setStage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

customExtensionHandlersCustomExtensionHandler2CustomExtension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler2CustomExtension.setId('219f57b6-7983-45a1-be01-2c228b7a43f8')


customExtensionHandlersCustomExtensionHandler2.setCustomExtension($customExtensionHandlersCustomExtensionHandler2CustomExtension)

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler2;
request_body.setCustomExtensionHandlers(customExtensionHandlersArray)


additionalData = [
'expiration' => request_body = Expiration()
request_body.setType('afterDuration')

request_body.setDuration('P365D')


request_body.setExpiration($expiration)

];
request_body.setAdditionalData(additionalData)




result = await client.identityGovernance_entitlementManagement_accessPackageAssignmentPolicies.post(request_body)


```
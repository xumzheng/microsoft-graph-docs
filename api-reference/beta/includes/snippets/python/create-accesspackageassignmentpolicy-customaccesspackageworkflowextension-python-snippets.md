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

customExtensionHandlersCustomExtensionHandler1 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler1.Stage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

customExtensionHandlersCustomExtensionHandler1CustomExtension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler1CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionHandlersCustomExtensionHandler1.customExtension = customExtensionHandlersCustomExtensionHandler1CustomExtension

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler1;
customExtensionHandlersCustomExtensionHandler2 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler2.Stage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

customExtensionHandlersCustomExtensionHandler2CustomExtension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler2CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionHandlersCustomExtensionHandler2.customExtension = customExtensionHandlersCustomExtensionHandler2CustomExtension

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler2;
request_body.customextensionhandlers(customExtensionHandlersArray)


additionalData = [
'expiration' => request_body = Expiration()
request_body.type = 'afterDuration'

request_body.duration = 'P365D'


request_body.expiration = expiration

];
request_body.additionaldata(additionalData)




request_configuration = AccessPackageAssignmentPoliciesRequestBuilderPostRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```
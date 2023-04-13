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

custom_extension_handlers_custom_extension_handler1 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler1.Stage(AccessPackageCustomExtensionStage('assignmentrequestcreated'))

custom_extension_handlers_custom_extension_handler1_custom_extension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler1CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionHandlersCustomExtensionHandler1.custom_extension = customExtensionHandlersCustomExtensionHandler1CustomExtension

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler1;
custom_extension_handlers_custom_extension_handler2 = CustomExtensionHandler()
customExtensionHandlersCustomExtensionHandler2.Stage(AccessPackageCustomExtensionStage('assignmentrequestgranted'))

custom_extension_handlers_custom_extension_handler2_custom_extension = CustomAccessPackageWorkflowExtension()
customExtensionHandlersCustomExtensionHandler2CustomExtension.id = '219f57b6-7983-45a1-be01-2c228b7a43f8'


customExtensionHandlersCustomExtensionHandler2.custom_extension = customExtensionHandlersCustomExtensionHandler2CustomExtension

customExtensionHandlersArray []= customExtensionHandlersCustomExtensionHandler2;
request_body.customextensionhandlers(customExtensionHandlersArray)


additionalData = [
'expiration' => request_body = Expiration()
request_body.type = 'afterDuration'

request_body.duration = 'P365D'


request_body.expiration = expiration

];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```
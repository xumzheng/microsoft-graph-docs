---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.id = '5540a08f-8ab5-43f6-a923-015275799197'

request_body.displayName = 'policy with access package custom workflow extension'

request_body.description = 'Run specified access package custom workflow extension at different stages.'

request_body.accessPackageId = 'ba5807c7-2aa9-4c8a-907e-4a17ee587500'

request_body.requestApprovalSettings=null

requestor_settings = RequestorSettings()
requestorSettings.accept_requests = True

requestorSettings.scopeType = 'AllExistingDirectorySubjects'

requestorSettings.AllowedRequestors([])


request_body.requestor_settings = requestorSettings
request_body.accessReviewSettings=null

request_body.CustomExtensionHandlers([])

additionalData = [
'expiration' => request_body = Expiration()
request_body.type = 'afterDuration'

request_body.duration = 'P365D'


request_body.expiration = expiration

];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body = request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.id = '4540a08f-8ab5-43f6-a923-015275799197'

request_body.displayName = 'policy with custom access package workflow extension'

request_body.description = 'Run specified custom access package workflow extension at different stages.'

request_body.accessPackageId = 'ba5807c7-2aa9-4c8a-907e-4a17ee587500'

request_body.requestApprovalSettings=null

requestorSettings = RequestorSettings()
requestorSettings.acceptRequests = true

requestorSettings.scopeType = 'AllExistingDirectorySubjects'

requestorSettings.AllowedRequestors([])


request_body.requestorSettings = requestorSettings
request_body.accessReviewSettings=null

request_body.CustomExtensionHandlers([])

additionalData = [
'expiration' => request_body = Expiration()
request_body.type = 'afterDuration'

request_body.duration = 'P365D'


request_body.expiration = expiration

];
request_body.additionaldata(additionalData)




request_configuration = AccessPackageAssignmentPolicyRequestBuilderPutRequestConfiguration(
)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body = request_body)


```
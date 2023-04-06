---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.setId('5540a08f-8ab5-43f6-a923-015275799197')

request_body.setDisplayName('policy with access package custom workflow extension')

request_body.setDescription('Run specified access package custom workflow extension at different stages.')

request_body.setAccessPackageId('ba5807c7-2aa9-4c8a-907e-4a17ee587500')

request_body.setRequestApprovalSettings(null)

requestorSettings = RequestorSettings()
requestorSettings.setAcceptRequests(true)

requestorSettings.setScopeType('AllExistingDirectorySubjects')

requestorSettings.setAllowedRequestors([])


request_body.setRequestorSettings($requestorSettings)
request_body.setAccessReviewSettings(null)

request_body.setCustomExtensionHandlers([])

additionalData = [
'expiration' => request_body = Expiration()
request_body.setType('afterDuration')

request_body.setDuration('P365D')


request_body.setExpiration($expiration)

];
request_body.setAdditionalData(additionalData)



request_config = AccessPackageAssignmentPolicyRequestBuilderPutRequestConfiguration(
request_config = AccessPackageAssignmentPolicyRequestBuilderPutRequestConfiguration(query_params=)


result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies_by_id('accessPackageAssignmentPolicy-id').put(request_body, headers=)


```
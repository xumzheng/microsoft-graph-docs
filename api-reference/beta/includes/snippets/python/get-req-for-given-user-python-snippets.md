---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetApplicablePolicyRequirementsPostRequestBody()
additionalData = [
'subject' => request_body = Subject()
		request_body.objectId = '5acd375c-8acb-45de-a958-fa0dd89259ad'


request_body.subject = subject

];
request_body.additionaldata(additionalData)





result = await client.identityGovernance.entitlementManagement.accessPackages_by_id('accessPackage-id').getApplicablePolicyRequirements.post(request_body = request_body)


```
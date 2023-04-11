---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MobilityManagementPolicy()
request_body.@odatatype = '#microsoft.graph.mobilityManagementPolicy'

request_body.complianceUrl = 'https://portal.mg.contoso.com/?portalAction=Compliance'

request_body.discoveryUrl = 'https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc'

request_body.termsOfUseUrl = 'https://portal.mg.contoso.com/TermsofUse.aspx'



request_configuration = MobilityManagementPolicyRequestBuilderPatchRequestConfiguration(
)


result = await client.policies.mobileAppManagementPolicies_by_id('mobilityManagementPolicy-id').patch(request_body = request_body)


```
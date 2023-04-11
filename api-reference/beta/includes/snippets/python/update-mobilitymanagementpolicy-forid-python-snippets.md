---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MobilityManagementPolicy()
request_body.@odatatype = '#microsoft.graph.mobilityManagementPolicy'

request_body.complianceUrl = 'https://portal.uem.contoso.com/?portalAction=Compliance'

request_body.discoveryUrl = 'https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc'

request_body.termsOfUseUrl = 'https://portal.uem.contoso.com/TermsofUse.aspx'




result = await client.policies.mobileDeviceManagementPolicies_by_id('mobilityManagementPolicy-id').patch(request_body = request_body)


```
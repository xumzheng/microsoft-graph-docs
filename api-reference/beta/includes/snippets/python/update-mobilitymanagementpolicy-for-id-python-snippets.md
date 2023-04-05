---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MobilityManagementPolicy()
request_body.set@odatatype('#microsoft.graph.mobilityManagementPolicy')

request_body.setComplianceUrl('https://portal.mg.contoso.com/?portalAction=Compliance')

request_body.setDiscoveryUrl('https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc')

request_body.setTermsOfUseUrl('https://portal.mg.contoso.com/TermsofUse.aspx')



result = await client.policies.mobileAppManagementPoliciesby_id('mobilityManagementPolicy-id').patch(request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MobilityManagementPolicy();
$requestBody.set@odatatype('#microsoft.graph.mobilityManagementPolicy');

$requestBody.setComplianceUrl('https://portal.mg.contoso.com/?portalAction=Compliance');

$requestBody.setDiscoveryUrl('https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc');

$requestBody.setTermsOfUseUrl('https://portal.mg.contoso.com/TermsofUse.aspx');



$requestResult = $graphServiceClient.policies().mobileAppManagementPoliciesById('mobilityManagementPolicy-id').patch($requestBody);


```
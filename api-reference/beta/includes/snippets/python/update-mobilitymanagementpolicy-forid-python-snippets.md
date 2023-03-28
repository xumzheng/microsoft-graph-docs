---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MobilityManagementPolicy();
$requestBody->set@odatatype('#microsoft.graph.mobilityManagementPolicy');

$requestBody->setComplianceUrl('https://portal.uem.contoso.com/?portalAction=Compliance');

$requestBody->setDiscoveryUrl('https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc');

$requestBody->setTermsOfUseUrl('https://portal.uem.contoso.com/TermsofUse.aspx');



$requestResult = $graphServiceClient->policies()->mobileDeviceManagementPoliciesById('mobilityManagementPolicy-id')->patch($requestBody);


```
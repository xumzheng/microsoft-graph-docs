---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MobilityManagementPolicy();


$requestRequestBody->setComplianceUrl('https://portal.uem.contoso.com/?portalAction=Compliance');
$requestRequestBody->setDiscoveryUrl('https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc');
$requestRequestBody->setTermsOfUseUrl('https://portal.uem.contoso.com/TermsofUse.aspx');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.mobilityManagementPolicy',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->policies()->mobileDeviceManagementPoliciesById('mobilityManagementPolicy-id')->patch($requestRequestBody);


```
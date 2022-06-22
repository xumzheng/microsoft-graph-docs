---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Alert();


$requestRequestBody->setAssignedTo('String');
$requestRequestBody->setClosedDateTime(new DateTime("String (timestamp)"));
$requestRequestBody->setComments( [
'String',],
$requestRequestBody->setFeedback(new AlertFeedback('@odata.type: microsoft.graph.alertFeedback'));
$requestRequestBody->setStatus(new AlertStatus('@odata.type: microsoft.graph.alertStatus'));
$requestRequestBody->setTags( [
'String',],

$vendorInformation = new SecurityVendorInformation();
$requestRequestBody->setVendorInformation($vendorInformation);


$vendorInformation->setProvider('String');
$vendorInformation->setVendor('String');

$requestConfiguration = new AlertRequestBuilderPatchRequestConfiguration();

$headers = [
"Prefer" => "return=representation",
];

$requestConfiguration->headers = $headers;


$result =  $graphClient->security()->alertsById('alert-id')->patch($requestRequestBody, $requestConfiguration);


```
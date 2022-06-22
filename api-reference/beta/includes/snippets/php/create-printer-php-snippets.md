---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CreatePostRequestBody();


$requestRequestBody->setDisplayName('Test Printer');
$requestRequestBody->setManufacturer('Test Printer Manufacturer');
$requestRequestBody->setModel('Test Printer Model');
$requestRequestBody->setPhysicalDeviceId(null);
$requestRequestBody->setHasPhysicalDevice(False);

$certificateSigningRequest = new PrintCertificateSigningRequest();
$requestRequestBody->setCertificateSigningRequest($certificateSigningRequest);


$certificateSigningRequest->setContent('{content}');
$certificateSigningRequest->setTransportKey('{sampleTransportKey}');

$requestRequestBody->setConnectorId(null);
$result =  $graphClient->print()->printers()->create()->post($requestRequestBody);


```
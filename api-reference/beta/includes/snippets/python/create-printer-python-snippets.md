---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CreatePostRequestBody();
requestBody.setDisplayName('Test Printer');

requestBody.setManufacturer('Test Printer Manufacturer');

requestBody.setModel('Test Printer Model');

requestBody.setPhysicalDeviceId(null);

requestBody.setHasPhysicalDevice(false);

certificateSigningRequest = PrintCertificateSigningRequest();
certificateSigningRequest.setContent('{content}');

certificateSigningRequest.setTransportKey('{sampleTransportKey}');


requestBody.setCertificateSigningRequest($certificateSigningRequest);
requestBody.setConnectorId(null);



graphServiceClient.print().printers().create().post(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreatePostRequestBody()
request_body.setDisplayName('Test Printer')

request_body.setManufacturer('Test Printer Manufacturer')

request_body.setModel('Test Printer Model')

request_body.setPhysicalDeviceId(null)

request_body.setHasPhysicalDevice(false)

certificateSigningRequest = PrintCertificateSigningRequest()
certificateSigningRequest.setContent('{content}')

certificateSigningRequest.setTransportKey('{sampleTransportKey}')


request_body.setCertificateSigningRequest($certificateSigningRequest)
request_body.setConnectorId(null)


request_config = CreateRequestBuilderPostRequestConfiguration(
request_config = CreateRequestBuilderPostRequestConfiguration(query_params=)


await client.print.printers.create.post(request_body, headers=)


```
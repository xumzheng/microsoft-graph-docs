---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CreatePostRequestBody()
request_body.displayName = 'Test Printer'

request_body.manufacturer = 'Test Printer Manufacturer'

request_body.model = 'Test Printer Model'

request_body.physicalDeviceId=null

request_body.hasPhysicalDevice = false

certificateSigningRequest = PrintCertificateSigningRequest()
certificateSigningRequest.content = '{content}'

certificateSigningRequest.transportKey = '{sampleTransportKey}'


request_body.certificateSigningRequest = certificateSigningRequest
request_body.connectorId=null



request_configuration = CreateRequestBuilderPostRequestConfiguration(
)


await client.print.printers.create.post(request_body = request_body)


```
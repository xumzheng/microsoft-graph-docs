---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Alert()
request_body.setAssignedTo('String')

request_body.setClosedDateTime(DateTime('String (timestamp)'))

request_body.setComments(['String', ])

request_body.setFeedback(AlertFeedback('alertfeedback'))

request_body.setStatus(AlertStatus('alertstatus'))

request_body.setTags(['String', ])

vendorInformation = SecurityVendorInformation()
vendorInformation.setProvider('String')

vendorInformation.setVendor('String')


request_body.setVendorInformation($vendorInformation)

request_config = AlertRequestBuilderPatchRequestConfiguration()

headers = [
'Prefer' => 'return=representation',
]

request_config.headers = headers


result = await client.security.alertsById('alert-id').patch(request_body, request_config)


```
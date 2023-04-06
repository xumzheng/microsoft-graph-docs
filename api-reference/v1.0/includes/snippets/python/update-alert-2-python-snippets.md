---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

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

request_config = AlertRequestBuilderPatchRequestConfiguration(
request_config = AlertRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"


result = await client.security.alerts_by_id('alert-id').patch(request_body, request_config, headers=request_config)


```
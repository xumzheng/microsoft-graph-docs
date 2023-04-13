---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Alert()
request_body.assignedTo = 'String'

request_body.closedDateTime = DateTime('String (timestamp)')

request_body.Comments(['String', ])

request_body.Feedback(AlertFeedback('alertfeedback'))

request_body.Status(AlertStatus('alertstatus'))

request_body.Tags(['String', ])

vendor_information = SecurityVendorInformation()
vendorInformation.provider = 'String'

vendorInformation.vendor = 'String'


request_body.vendor_information = vendorInformation



result = await client.security.alerts_by_id('alert-id').patch(request_body = request_body)


```
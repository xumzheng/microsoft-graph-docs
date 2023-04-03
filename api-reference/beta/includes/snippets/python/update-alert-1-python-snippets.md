---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Alert();
requestBody.setAssignedTo('String');

requestBody.setClosedDateTime(DateTime('String (timestamp)'));

requestBody.setComments(['String', ]);

requestBody.setFeedback(AlertFeedback('alertfeedback'));

requestBody.setStatus(AlertStatus('alertstatus'));

requestBody.setTags(['String', ]);

vendorInformation = SecurityVendorInformation();
vendorInformation.setProvider('String');

vendorInformation.setVendor('String');


requestBody.setVendorInformation($vendorInformation);


requestResult = graphServiceClient.security().alertsById('alert-id').patch(requestBody);


```
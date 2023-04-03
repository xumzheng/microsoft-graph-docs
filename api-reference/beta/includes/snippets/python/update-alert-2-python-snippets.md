---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

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

request_config = AlertRequestBuilderPatchRequestConfiguration();

headers = [
'Prefer' => 'return=representation',
];

request_config.headers = headers;


result = await client.security().alertsById('alert-id').patch(requestBody, request_config);


```
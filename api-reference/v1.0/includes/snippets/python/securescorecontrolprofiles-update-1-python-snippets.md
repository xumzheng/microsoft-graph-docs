---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = SecureScoreControlProfile();
vendorInformation = SecurityVendorInformation();
vendorInformation.setProvider('SecureScore');

VendorInformation.setProviderVersion(null);

VendorInformation.setSubProvider(null);

vendorInformation.setVendor('Microsoft');


requestBody.setVendorInformation($vendorInformation);
additionalData = [
'assignedTo' => '', 
'comment' => 'control is reviewed', 
'state' => 'Reviewed', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.security().secureScoreControlProfilesById('secureScoreControlProfile-id').patch(requestBody);


```
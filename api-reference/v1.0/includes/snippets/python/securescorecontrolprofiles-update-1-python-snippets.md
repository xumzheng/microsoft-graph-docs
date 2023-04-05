---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SecureScoreControlProfile()
vendorInformation = SecurityVendorInformation()
vendorInformation.setProvider('SecureScore')

VendorInformation.setProviderVersion(null)

VendorInformation.setSubProvider(null)

vendorInformation.setVendor('Microsoft')


request_body.setVendorInformation($vendorInformation)
additionalData = [
'assignedTo' => '', 
'comment' => 'control is reviewed', 
'state' => 'Reviewed', 
];
request_body.setAdditionalData(additionalData)




result = await client.security.secureScoreControlProfilesById('secureScoreControlProfile-id').patch(request_body)


```
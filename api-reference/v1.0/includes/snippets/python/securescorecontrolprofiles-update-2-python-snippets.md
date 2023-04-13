---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SecureScoreControlProfile()
vendor_information = SecurityVendorInformation()
vendorInformation.provider = 'SecureScore'

VendorInformation.providerVersion=null

VendorInformation.subProvider=null

vendorInformation.vendor = 'Microsoft'


request_body.vendor_information = vendorInformation
additionalData = [
'assignedTo' => '', 
'comment' => 'control is reviewed', 
'state' => 'Reviewed', 
];
request_body.additionaldata(additionalData)





result = await client.security.secureScoreControlProfiles_by_id('secureScoreControlProfile-id').patch(request_body = request_body)


```
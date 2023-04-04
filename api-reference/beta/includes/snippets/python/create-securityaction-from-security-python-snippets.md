---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = SecurityAction()
request_body.setName('BlockIp')

request_body.setActionReason('Test')

parametersKeyValuePair1 = KeyValuePair()
parametersKeyValuePair1.setName('IP')

parametersKeyValuePair1.setValue('1.2.3.4')


parametersArray []= parametersKeyValuePair1;
request_body.setParameters(parametersArray)


vendorInformation = SecurityVendorInformation()
vendorInformation.setProvider('Windows Defender ATP')

vendorInformation.setVendor('Microsoft')


request_body.setVendorInformation($vendorInformation)


result = await client.security.securityActions.post(request_body)


```
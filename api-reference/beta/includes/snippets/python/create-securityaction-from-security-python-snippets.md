---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SecurityAction()
request_body.name = 'BlockIp'

request_body.actionReason = 'Test'

parametersKeyValuePair1 = KeyValuePair()
parametersKeyValuePair1.name = 'IP'

parametersKeyValuePair1.value = '1.2.3.4'


parametersArray []= parametersKeyValuePair1;
request_body.parameters(parametersArray)


vendorInformation = SecurityVendorInformation()
vendorInformation.provider = 'Windows Defender ATP'

vendorInformation.vendor = 'Microsoft'


request_body.vendorInformation = vendorInformation


request_configuration = SecurityActionsRequestBuilderPostRequestConfiguration(
)


result = await client.security.securityActions.post(request_body = request_body)


```
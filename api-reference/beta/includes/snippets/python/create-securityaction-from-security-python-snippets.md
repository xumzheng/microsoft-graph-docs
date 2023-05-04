---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Security_action()
request_body.name = 'BlockIp'

request_body.action_reason = 'Test'

parameters_key_value_pair1 = Key_value_pair()
parameters_key_value_pair1.name = 'IP'

parameters_key_value_pair1.value = '1.2.3.4'


parametersArray []= parametersKeyValuePair1;
request_body.parameters(parametersArray)


vendor_information = Security_vendor_information()
vendor_information.provider = 'Windows Defender ATP'

vendor_information.vendor = 'Microsoft'


request_body.vendor_information = vendor_information



result = await client.security.security_actions.post(request_body = request_body)


```
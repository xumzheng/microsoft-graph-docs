---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.set@odatatype('#microsoft.graph.ipNamedLocation')

request_body.setDisplayName('Untrusted named location with only IPv4 address')

additionalData = [
'isTrusted' => false,
'ipRanges' => ipRanges1 = ()
		ipRanges1.set@odatatype('#microsoft.graph.iPv4CidrRange')

		ipRanges1.setCidrAddress('6.5.4.3/18')


ipRangesArray []= ipRanges1;
request_body.setIpRanges(ipRangesArray)


];
request_body.setAdditionalData(additionalData)




result = await client.identity_conditionalAccess_namedLocationsby_id('namedLocation-id').patch(request_body)


```
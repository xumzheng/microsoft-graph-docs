---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odatatype = '#microsoft.graph.ipNamedLocation'

request_body.displayName = 'Untrusted named location with only IPv4 address'

additionalData = [
'isTrusted' => false,
'ipRanges' => ipRanges1 = ()
		ipRanges1.@odatatype = '#microsoft.graph.iPv4CidrRange'

		ipRanges1.cidrAddress = '6.5.4.3/18'


ipRangesArray []= ipRanges1;
request_body.ipranges(ipRangesArray)


];
request_body.additionaldata(additionalData)





result = await client.identity.conditionalAccess.namedLocations_by_id('namedLocation-id').patch(request_body = request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NamedLocation()
request_body.@odatatype = '#microsoft.graph.ipNamedLocation'

request_body.displayName = 'Untrusted IP named location'

additionalData = [
'isTrusted' => false,
'ipRanges' => ipRanges1 = ()
		ipRanges1.@odatatype = '#microsoft.graph.iPv4CidrRange'

		ipRanges1.cidrAddress = '12.34.221.11/22'


ipRangesArray []= ipRanges1;
ipRanges2 = ()
		ipRanges2.@odatatype = '#microsoft.graph.iPv6CidrRange'

		ipRanges2.cidrAddress = '2001:0:9d38:90d6:0:0:0:0/63'


ipRangesArray []= ipRanges2;
request_body.ipranges(ipRangesArray)


];
request_body.additionaldata(additionalData)




request_configuration = NamedLocationsRequestBuilderPostRequestConfiguration(
)


result = await client.identity.conditionalAccess.namedLocations.post(request_body = request_body)


```
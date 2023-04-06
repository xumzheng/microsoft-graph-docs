---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TiIndicator()
request_body.setAction(TiAction('alert'))

request_body.setActivityGroupNames([])

request_body.setConfidence(0)

request_body.setDescription('This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.')

request_body.setExpirationDateTime(DateTime('2019-03-01T21:43:37.5031462+00:00'))

request_body.setExternalId('Test--8586509942679764298MS501')

request_body.setFileHashType(FileHashType('sha256'))

request_body.setFileHashValue('aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313')

request_body.setKillChain([])

request_body.setMalwareFamilyNames([])

request_body.setSeverity(0)

request_body.setTags([])

request_body.setTargetProduct('Azure Sentinel')

request_body.setThreatType('WatchList')

request_body.setTlpLevel(TlpLevel('green'))


request_config = TiIndicatorsRequestBuilderPostRequestConfiguration(
request_config = TiIndicatorsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.tiIndicators.post(request_body, headers=)


```
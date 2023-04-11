---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SubmitTiIndicatorsPostRequestBody()
valueTiIndicator1 = TiIndicator()
valueTiIndicator1.ActivityGroupNames([])

valueTiIndicator1.confidence = 0

valueTiIndicator1.description = 'This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.'

valueTiIndicator1.expirationDateTime = DateTime('2019-03-01T21:44:03.1668987+00:00')

valueTiIndicator1.externalId = 'Test--8586509942423126760MS164-0'

valueTiIndicator1.FileHashType(FileHashType('sha256'))

valueTiIndicator1.fileHashValue = 'b555c45c5b1b01304217e72118d6ca1b14b7013644a078273cea27bbdc1cf9d6'

valueTiIndicator1.KillChain([])

valueTiIndicator1.MalwareFamilyNames([])

valueTiIndicator1.severity = 0

valueTiIndicator1.Tags([])

valueTiIndicator1.targetProduct = 'Azure Sentinel'

valueTiIndicator1.threatType = 'WatchList'

valueTiIndicator1.TlpLevel(TlpLevel('green'))


valueArray []= valueTiIndicator1;
valueTiIndicator2 = TiIndicator()
valueTiIndicator2.ActivityGroupNames([])

valueTiIndicator2.confidence = 0

valueTiIndicator2.description = 'This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.'

valueTiIndicator2.expirationDateTime = DateTime('2019-03-01T21:44:03.1748779+00:00')

valueTiIndicator2.externalId = 'Test--8586509942423126760MS164-1'

valueTiIndicator2.FileHashType(FileHashType('sha256'))

valueTiIndicator2.fileHashValue = '1796b433950990b28d6a22456c9d2b58ced1bdfcdf5f16f7e39d6b9bdca4213b'

valueTiIndicator2.KillChain([])

valueTiIndicator2.MalwareFamilyNames([])

valueTiIndicator2.severity = 0

valueTiIndicator2.Tags([])

valueTiIndicator2.targetProduct = 'Azure Sentinel'

valueTiIndicator2.threatType = 'WatchList'

valueTiIndicator2.TlpLevel(TlpLevel('green'))


valueArray []= valueTiIndicator2;
request_body.value(valueArray)




request_configuration = SubmitTiIndicatorsRequestBuilderPostRequestConfiguration(
)


result = await client.security.tiIndicators.submitTiIndicators.post(request_body = request_body)


```
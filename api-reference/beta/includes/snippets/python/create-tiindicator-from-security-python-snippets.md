---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = TiIndicator();
requestBody.setAction(TiAction('alert'));

requestBody.setActivityGroupNames([]);

requestBody.setConfidence(0);

requestBody.setDescription('This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.');

requestBody.setExpirationDateTime(DateTime('2019-03-01T21:43:37.5031462+00:00'));

requestBody.setExternalId('Test--8586509942679764298MS501');

requestBody.setFileHashType(FileHashType('sha256'));

requestBody.setFileHashValue('aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313');

requestBody.setKillChain([]);

requestBody.setMalwareFamilyNames([]);

requestBody.setSeverity(0);

requestBody.setTags([]);

requestBody.setTargetProduct('Azure Sentinel');

requestBody.setThreatType('WatchList');

requestBody.setTlpLevel(TlpLevel('green'));



result = awaitclient.security().tiIndicators().post(requestBody);


```
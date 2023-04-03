---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AcquireAccessTokenPostRequestBody();
credentialsSynchronizationSecretKeyStringValuePair1 = SynchronizationSecretKeyStringValuePair();
credentialsSynchronizationSecretKeyStringValuePair1.set@odatatype('microsoft.graph.synchronizationSecretKeyStringValuePair');


credentialsArray []= credentialsSynchronizationSecretKeyStringValuePair1;
requestBody.setCredentials(credentialsArray);




awaitclient.applicationsById('application-id').synchronization().acquireAccessToken().post(requestBody);


```
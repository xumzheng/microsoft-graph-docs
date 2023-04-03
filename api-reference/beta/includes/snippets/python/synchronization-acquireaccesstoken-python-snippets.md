---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AcquireAccessTokenPostRequestBody();
credentialsSynchronizationSecretKeyStringValuePair1 = SynchronizationSecretKeyStringValuePair();
credentialsSynchronizationSecretKeyStringValuePair1.set@odatatype('microsoft.graph.synchronizationSecretKeyStringValuePair');


credentialsArray []= credentialsSynchronizationSecretKeyStringValuePair1;
requestBody.setCredentials(credentialsArray);




await client.applicationsById('application-id').synchronization().acquireAccessToken().post(requestBody);


```
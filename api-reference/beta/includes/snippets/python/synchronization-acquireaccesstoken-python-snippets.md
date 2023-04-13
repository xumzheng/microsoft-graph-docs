---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AcquireAccessTokenPostRequestBody()
credentials_synchronization_secret_key_string_value_pair1 = SynchronizationSecretKeyStringValuePair()
credentialsSynchronizationSecretKeyStringValuePair1.@odatatype = 'microsoft.graph.synchronizationSecretKeyStringValuePair'


credentialsArray []= credentialsSynchronizationSecretKeyStringValuePair1;
request_body.credentials(credentialsArray)





await client.applications_by_id('application-id').synchronization.acquireAccessToken.post(request_body = request_body)


```
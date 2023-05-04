---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Acquire_access_token_post_request_body()
credentials_synchronization_secret_key_string_value_pair1 = Synchronization_secret_key_string_value_pair()
credentials_synchronization_secret_key_string_value_pair1.@odata_type = 'microsoft.graph.synchronizationSecretKeyStringValuePair'


credentialsArray []= credentialsSynchronizationSecretKeyStringValuePair1;
request_body.credentials(credentialsArray)





await client.applications.by_application_id('application-id').synchronization.acquire_acces_token.post(request_body = request_body)


```
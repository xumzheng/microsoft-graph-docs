---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new AcquireAccessTokenPostRequestBody();
$credentialsSynchronizationSecretKeyStringValuePair1 = new SynchronizationSecretKeyStringValuePair();
$credentialsSynchronizationSecretKeyStringValuePair1->set@odatatype('microsoft.graph.synchronizationSecretKeyStringValuePair');


$credentialsArray []= $credentialsSynchronizationSecretKeyStringValuePair1;
$requestBody->setCredentials($credentialsArray);




$graphServiceClient->applicationsById('application-id')->synchronization()->acquireAccessToken()->post($requestBody);


```
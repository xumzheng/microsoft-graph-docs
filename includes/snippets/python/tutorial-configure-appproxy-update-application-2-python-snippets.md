---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Application();
onPremisesPublishing = OnPremisesPublishing();
onPremisesPublishing.setExternalAuthenticationType(ExternalAuthenticationType('aadpreauthentication'));

onPremisesPublishing.setInternalUrl('https://contosoiwaapp.com');

onPremisesPublishing.setExternalUrl('https://contosoiwaapp-contoso.msappproxy.net');

onPremisesPublishing.setIsHttpOnlyCookieEnabled(true);

onPremisesPublishing.setIsOnPremPublishingEnabled(true);

onPremisesPublishing.setIsPersistentCookieEnabled(true);

onPremisesPublishing.setIsSecureCookieEnabled(true);

onPremisesPublishing.setIsStateSessionEnabled(true);

onPremisesPublishing.setIsTranslateHostHeaderEnabled(true);

onPremisesPublishing.setIsTranslateLinksInBodyEnabled(true);


requestBody.setOnPremisesPublishing($onPremisesPublishing);


requestResult = graphServiceClient.applicationsById('application-id').patch(requestBody);


```
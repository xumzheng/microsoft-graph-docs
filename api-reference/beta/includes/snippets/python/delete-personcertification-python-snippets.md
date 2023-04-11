---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = PersonCertificationRequestBuilderDeleteRequestConfiguration(
)


await client.users_by_id('user-id').profile.certifications_by_id('personCertification-id').delete()


```
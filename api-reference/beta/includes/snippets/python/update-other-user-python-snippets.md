---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = User();
requestBody.setBusinessPhones(['+1 425 555 0109', ]);

requestBody.setOfficeLocation('18/2111');

authorizationInfo = AuthorizationInfo();
authorizationInfo.setCertificateUserIds(['5432109876543210@mil', ]);


requestBody.setAuthorizationInfo($authorizationInfo);


result = awaitclient.usersById('user-id').patch(requestBody);


```
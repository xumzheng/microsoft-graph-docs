---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Organization();
requestBody.setMarketingNotificationEmails(['marketing@contoso.com', ]);

privacyProfile = PrivacyProfile();
privacyProfile.setContactEmail('alice@contoso.com');

privacyProfile.setStatementUrl('https://contoso.com/privacyStatement');


requestBody.setPrivacyProfile($privacyProfile);
requestBody.setSecurityComplianceNotificationMails(['security@contoso.com', ]);

requestBody.setSecurityComplianceNotificationPhones(['(123) 456-7890', ]);

requestBody.setTechnicalNotificationMails(['tech@contoso.com', ]);



requestResult = graphServiceClient.organizationById('organization-id').patch(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Organization()
request_body.setMarketingNotificationEmails(['marketing@contoso.com', ])

privacyProfile = PrivacyProfile()
privacyProfile.setContactEmail('alice@contoso.com')

privacyProfile.setStatementUrl('https://contoso.com/privacyStatement')


request_body.setPrivacyProfile($privacyProfile)
request_body.setSecurityComplianceNotificationMails(['security@contoso.com', ])

request_body.setSecurityComplianceNotificationPhones(['(123) 456-7890', ])

request_body.setTechnicalNotificationMails(['tech@contoso.com', ])


request_config = OrganizationRequestBuilderPatchRequestConfiguration(
request_config = OrganizationRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.organization_by_id('organization-id').patch(request_body, headers=)


```
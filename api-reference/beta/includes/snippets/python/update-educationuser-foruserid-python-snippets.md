---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationUser()
relatedContactsRelatedContact1 = RelatedContact()
relatedContactsRelatedContact1.displayName = 'Father Time'

relatedContactsRelatedContact1.emailAddress = 'father@time.com'

relatedContactsRelatedContact1.mobilePhone = '4251231234'

relatedContactsRelatedContact1.Relationship(ContactRelationship('guardian'))

relatedContactsRelatedContact1.accessConsent = true


relatedContactsArray []= relatedContactsRelatedContact1;
relatedContactsRelatedContact2 = RelatedContact()
relatedContactsRelatedContact2.displayName = 'Mother Nature'

relatedContactsRelatedContact2.emailAddress = 'mother@nature.co.uk'

relatedContactsRelatedContact2.mobilePhone = '3251231234'

relatedContactsRelatedContact2.Relationship(ContactRelationship('parent'))

relatedContactsRelatedContact2.accessConsent = true


relatedContactsArray []= relatedContactsRelatedContact2;
request_body.relatedcontacts(relatedContactsArray)





result = await client.education.users_by_id('educationUser-id').patch(request_body = request_body)


```
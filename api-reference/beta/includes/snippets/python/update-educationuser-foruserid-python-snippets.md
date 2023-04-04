---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationUser()
relatedContactsRelatedContact1 = RelatedContact()
relatedContactsRelatedContact1.setDisplayName('Father Time')

relatedContactsRelatedContact1.setEmailAddress('father@time.com')

relatedContactsRelatedContact1.setMobilePhone('4251231234')

relatedContactsRelatedContact1.setRelationship(ContactRelationship('guardian'))

relatedContactsRelatedContact1.setAccessConsent(true)


relatedContactsArray []= relatedContactsRelatedContact1;
relatedContactsRelatedContact2 = RelatedContact()
relatedContactsRelatedContact2.setDisplayName('Mother Nature')

relatedContactsRelatedContact2.setEmailAddress('mother@nature.co.uk')

relatedContactsRelatedContact2.setMobilePhone('3251231234')

relatedContactsRelatedContact2.setRelationship(ContactRelationship('parent'))

relatedContactsRelatedContact2.setAccessConsent(true)


relatedContactsArray []= relatedContactsRelatedContact2;
request_body.setRelatedContacts(relatedContactsArray)




result = await client.education.usersById('educationUser-id').patch(request_body)


```
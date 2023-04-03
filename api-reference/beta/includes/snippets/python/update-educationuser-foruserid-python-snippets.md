---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = EducationUser();
relatedContactsRelatedContact1 = RelatedContact();
relatedContactsRelatedContact1.setDisplayName('Father Time');

relatedContactsRelatedContact1.setEmailAddress('father@time.com');

relatedContactsRelatedContact1.setMobilePhone('4251231234');

relatedContactsRelatedContact1.setRelationship(ContactRelationship('guardian'));

relatedContactsRelatedContact1.setAccessConsent(true);


relatedContactsArray []= relatedContactsRelatedContact1;
relatedContactsRelatedContact2 = RelatedContact();
relatedContactsRelatedContact2.setDisplayName('Mother Nature');

relatedContactsRelatedContact2.setEmailAddress('mother@nature.co.uk');

relatedContactsRelatedContact2.setMobilePhone('3251231234');

relatedContactsRelatedContact2.setRelationship(ContactRelationship('parent'));

relatedContactsRelatedContact2.setAccessConsent(true);


relatedContactsArray []= relatedContactsRelatedContact2;
requestBody.setRelatedContacts(relatedContactsArray);




requestResult = graphServiceClient.education().usersById('educationUser-id').patch(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationUser()
request_body.displayName = 'Dion Matheson'

request_body.givenName = 'Dion'

request_body.middleName=null

request_body.surname = 'Matheson'

request_body.mail = 'DionM@contoso.com'

request_body.mobilePhone = '+1 (253) 555-0101'

created_by = IdentitySet()
created_by_user = Identity()
createdByUser.displayName = 'Susana Rocha'

createdByUser.id = '14012'


createdBy.user = createdByUser

request_body.created_by = createdBy
request_body.ExternalSource(EducationExternalSource('sis'))

mailing_address = PhysicalAddress()
mailingAddress.city = 'Los Angeles'

mailingAddress.countryOrRegion = 'United States'

mailingAddress.postalCode = '98055'

mailingAddress.state = 'CA'

mailingAddress.street = '12345 Main St.'


request_body.mailing_address = mailingAddress
request_body.PrimaryRole(EducationUserRole('student'))

residence_address = PhysicalAddress()
residenceAddress.city = 'Los Angeles'

residenceAddress.countryOrRegion = 'United States'

residenceAddress.postalCode = '98055'

residenceAddress.state = 'CA'

residenceAddress.street = '12345 Main St.'


request_body.residence_address = residenceAddress



result = await client.education.users.post(request_body = request_body)


```
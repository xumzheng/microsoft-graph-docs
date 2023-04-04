---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationUser();
request_body.setDisplayName('Dion Matheson');

request_body.setGivenName('Dion');

request_body.setMiddleName(null);

request_body.setSurname('Matheson');

request_body.setMail('DionM@contoso.com');

request_body.setMobilePhone('+1 (253) 555-0101');

createdBy = IdentitySet();
createdByUser = Identity();
createdByUser.setDisplayName('Susana Rocha');

createdByUser.setId('14012');


createdBy.setUser($createdByUser);

request_body.setCreatedBy($createdBy);
request_body.setExternalSource(EducationExternalSource('sis'));

mailingAddress = PhysicalAddress();
mailingAddress.setCity('Los Angeles');

mailingAddress.setCountryOrRegion('United States');

mailingAddress.setPostalCode('98055');

mailingAddress.setState('CA');

mailingAddress.setStreet('12345 Main St.');


request_body.setMailingAddress($mailingAddress);
request_body.setPrimaryRole(EducationUserRole('student'));

residenceAddress = PhysicalAddress();
residenceAddress.setCity('Los Angeles');

residenceAddress.setCountryOrRegion('United States');

residenceAddress.setPostalCode('98055');

residenceAddress.setState('CA');

residenceAddress.setStreet('12345 Main St.');


request_body.setResidenceAddress($residenceAddress);


result = await client.education.users.post(request_body);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationUser();
request_body.set@odatatype('#microsoft.graph.educationUser');

request_body.setPrimaryRole(EducationUserRole('string'));

request_body.setMiddleName('String');

request_body.setExternalSource(EducationExternalSource('string'));

request_body.setExternalSourceDetail('String');

residenceAddress = PhysicalAddress();
residenceAddress.set@odatatype('microsoft.graph.physicalAddress');


request_body.setResidenceAddress($residenceAddress);
mailingAddress = PhysicalAddress();
mailingAddress.set@odatatype('microsoft.graph.physicalAddress');


request_body.setMailingAddress($mailingAddress);
student = EducationStudent();
student.set@odatatype('microsoft.graph.educationStudent');


request_body.setStudent($student);
teacher = EducationTeacher();
teacher.set@odatatype('microsoft.graph.educationTeacher');


request_body.setTeacher($teacher);
createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


request_body.setCreatedBy($createdBy);
request_body.setAccountEnabled(boolean);

assignedLicensesAssignedLicense1 = AssignedLicense();
assignedLicensesAssignedLicense1.set@odatatype('microsoft.graph.assignedLicense');


assignedLicensesArray []= assignedLicensesAssignedLicense1;
request_body.setAssignedLicenses(assignedLicensesArray);


assignedPlansAssignedPlan1 = AssignedPlan();
assignedPlansAssignedPlan1.set@odatatype('microsoft.graph.assignedPlan');


assignedPlansArray []= assignedPlansAssignedPlan1;
request_body.setAssignedPlans(assignedPlansArray);


request_body.setBusinessPhones(['String', ]);

request_body.setDepartment('String');

request_body.setDisplayName('String');

request_body.setGivenName('String');

request_body.setMail('String');

request_body.setMailNickname('String');

request_body.setMobilePhone('String');

request_body.setPasswordPolicies('String');

passwordProfile = PasswordProfile();
passwordProfile.set@odatatype('microsoft.graph.passwordProfile');


request_body.setPasswordProfile($passwordProfile);
request_body.setOfficeLocation('String');

request_body.setPreferredLanguage('String');

provisionedPlansProvisionedPlan1 = ProvisionedPlan();
provisionedPlansProvisionedPlan1.set@odatatype('microsoft.graph.provisionedPlan');


provisionedPlansArray []= provisionedPlansProvisionedPlan1;
request_body.setProvisionedPlans(provisionedPlansArray);


request_body.setRefreshTokensValidFromDateTime(DateTime('String (timestamp)'));

request_body.setShowInAddressList(boolean);

request_body.setSurname('String');

request_body.setUsageLocation('String');

request_body.setUserPrincipalName('String');

request_body.setUserType('String');

onPremisesInfo = EducationOnPremisesInfo();
onPremisesInfo.set@odatatype('microsoft.graph.educationOnPremisesInfo');


request_body.setOnPremisesInfo($onPremisesInfo);


result = await client.education.users.post(request_body);


```
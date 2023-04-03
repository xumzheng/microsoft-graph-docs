---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EducationUser();
requestBody.set@odatatype('#microsoft.graph.educationUser');

requestBody.setPrimaryRole(EducationUserRole('string'));

requestBody.setMiddleName('String');

requestBody.setExternalSource(EducationExternalSource('string'));

requestBody.setExternalSourceDetail('String');

residenceAddress = PhysicalAddress();
residenceAddress.set@odatatype('microsoft.graph.physicalAddress');


requestBody.setResidenceAddress($residenceAddress);
mailingAddress = PhysicalAddress();
mailingAddress.set@odatatype('microsoft.graph.physicalAddress');


requestBody.setMailingAddress($mailingAddress);
student = EducationStudent();
student.set@odatatype('microsoft.graph.educationStudent');


requestBody.setStudent($student);
teacher = EducationTeacher();
teacher.set@odatatype('microsoft.graph.educationTeacher');


requestBody.setTeacher($teacher);
createdBy = IdentitySet();
createdBy.set@odatatype('microsoft.graph.identitySet');


requestBody.setCreatedBy($createdBy);
requestBody.setAccountEnabled(boolean);

assignedLicensesAssignedLicense1 = AssignedLicense();
assignedLicensesAssignedLicense1.set@odatatype('microsoft.graph.assignedLicense');


assignedLicensesArray []= assignedLicensesAssignedLicense1;
requestBody.setAssignedLicenses(assignedLicensesArray);


assignedPlansAssignedPlan1 = AssignedPlan();
assignedPlansAssignedPlan1.set@odatatype('microsoft.graph.assignedPlan');


assignedPlansArray []= assignedPlansAssignedPlan1;
requestBody.setAssignedPlans(assignedPlansArray);


requestBody.setBusinessPhones(['String', ]);

requestBody.setDepartment('String');

requestBody.setDisplayName('String');

requestBody.setGivenName('String');

requestBody.setMail('String');

requestBody.setMailNickname('String');

requestBody.setMobilePhone('String');

requestBody.setPasswordPolicies('String');

passwordProfile = PasswordProfile();
passwordProfile.set@odatatype('microsoft.graph.passwordProfile');


requestBody.setPasswordProfile($passwordProfile);
requestBody.setOfficeLocation('String');

requestBody.setPreferredLanguage('String');

provisionedPlansProvisionedPlan1 = ProvisionedPlan();
provisionedPlansProvisionedPlan1.set@odatatype('microsoft.graph.provisionedPlan');


provisionedPlansArray []= provisionedPlansProvisionedPlan1;
requestBody.setProvisionedPlans(provisionedPlansArray);


requestBody.setRefreshTokensValidFromDateTime(DateTime('String (timestamp)'));

requestBody.setShowInAddressList(boolean);

requestBody.setSurname('String');

requestBody.setUsageLocation('String');

requestBody.setUserPrincipalName('String');

requestBody.setUserType('String');

onPremisesInfo = EducationOnPremisesInfo();
onPremisesInfo.set@odatatype('microsoft.graph.educationOnPremisesInfo');


requestBody.setOnPremisesInfo($onPremisesInfo);


result = await client.education().users().post(requestBody);


```
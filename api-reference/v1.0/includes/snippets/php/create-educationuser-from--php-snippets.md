---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationUser();


$requestRequestBody->setPrimaryRole(new EducationUserRole('String'));
$requestRequestBody->setMiddleName('String');
$requestRequestBody->setExternalSource(new EducationExternalSource('String'));
$requestRequestBody->setExternalSourceDetail('String');

$residenceAddress = new PhysicalAddress();
$requestRequestBody->setResidenceAddress($residenceAddress);


$residenceAddressAdditionalData = [
	"@odata.type" => 'microsoft.graph.physicalAddress',
];
$residenceAddress->setAdditionalData($residenceAddressAdditionalData);


$mailingAddress = new PhysicalAddress();
$requestRequestBody->setMailingAddress($mailingAddress);


$mailingAddressAdditionalData = [
"@odata.type" => 'microsoft.graph.physicalAddress',
];
$mailingAddress->setAdditionalData($mailingAddressAdditionalData);


$student = new EducationStudent();
$requestRequestBody->setStudent($student);


$studentAdditionalData = [
"@odata.type" => 'microsoft.graph.educationStudent',
];
$student->setAdditionalData($studentAdditionalData);


$teacher = new EducationTeacher();
$requestRequestBody->setTeacher($teacher);


$teacherAdditionalData = [
"@odata.type" => 'microsoft.graph.educationTeacher',
];
$teacher->setAdditionalData($teacherAdditionalData);


$createdBy = new IdentitySet();
$requestRequestBody->setCreatedBy($createdBy);


$createdByAdditionalData = [
"@odata.type" => 'microsoft.graph.identitySet',
];
$createdBy->setAdditionalData($createdByAdditionalData);

$requestRequestBody->setAccountEnabled('Boolean');
$assignedLicensesArray = [];

$assignedLicensesassignedLicenses1 = new AssignedLicense();

$assignedLicensesassignedLicenses1AdditionalData = [
"@odata.type" => 'microsoft.graph.assignedLicense',
];
$assignedLicensesassignedLicenses1->setAdditionalData($assignedLicensesassignedLicenses1AdditionalData);

$assignedLicensesArray []= $assignedLicensesassignedLicenses1;
$requestRequestBody->setAssignedLicenses($assignedLicensesArray);
$assignedPlansArray = [];

$assignedPlansassignedPlans1 = new AssignedPlan();

$assignedPlansassignedPlans1AdditionalData = [
"@odata.type" => 'microsoft.graph.assignedPlan',
];
$assignedPlansassignedPlans1->setAdditionalData($assignedPlansassignedPlans1AdditionalData);

$assignedPlansArray []= $assignedPlansassignedPlans1;
$requestRequestBody->setAssignedPlans($assignedPlansArray);
$requestRequestBody->setBusinessPhones(['String',]);
$requestRequestBody->setDepartment('String');
$requestRequestBody->setDisplayName('String');
$requestRequestBody->setGivenName('String');
$requestRequestBody->setMail('String');
$requestRequestBody->setMailNickname('String');
$requestRequestBody->setMobilePhone('String');
$requestRequestBody->setPasswordPolicies('String');

$passwordProfile = new PasswordProfile();
$requestRequestBody->setPasswordProfile($passwordProfile);


$passwordProfileAdditionalData = [
"@odata.type" => 'microsoft.graph.passwordProfile',
];
$passwordProfile->setAdditionalData($passwordProfileAdditionalData);

$requestRequestBody->setOfficeLocation('String');
$requestRequestBody->setPreferredLanguage('String');
$provisionedPlansArray = [];

$provisionedPlansprovisionedPlans1 = new ProvisionedPlan();

$provisionedPlansprovisionedPlans1AdditionalData = [
"@odata.type" => 'microsoft.graph.provisionedPlan',
];
$provisionedPlansprovisionedPlans1->setAdditionalData($provisionedPlansprovisionedPlans1AdditionalData);

$provisionedPlansArray []= $provisionedPlansprovisionedPlans1;
$requestRequestBody->setProvisionedPlans($provisionedPlansArray);
$requestRequestBody->setRefreshTokensValidFromDateTime(new DateTime("String (timestamp)"));
$requestRequestBody->setShowInAddressList('Boolean');
$requestRequestBody->setSurname('String');
$requestRequestBody->setUsageLocation('String');
$requestRequestBody->setUserPrincipalName('String');
$requestRequestBody->setUserType('String');

$onPremisesInfo = new EducationOnPremisesInfo();
$requestRequestBody->setOnPremisesInfo($onPremisesInfo);


$onPremisesInfoAdditionalData = [
"@odata.type" => 'microsoft.graph.educationOnPremisesInfo',
];
$onPremisesInfo->setAdditionalData($onPremisesInfoAdditionalData);

$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.educationUser',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->education()->users()->post($requestRequestBody);


```
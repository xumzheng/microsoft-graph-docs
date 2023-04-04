---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessPackageAssignmentPolicy();
request_body.setId('b2eba9a1-b357-42ee-83a8-336522ed6cbf');

request_body.setAccessPackageId('4c02f928-7752-49aa-8fc8-e286d973a965');

request_body.setDisplayName('All Users');

request_body.setDescription('All users can request for access to the directory.');

request_body.setCanExtend(false);

request_body.setDurationInDays(365);

request_body.setExpirationDateTime(null);

requestorSettings = RequestorSettings();
requestorSettings.setScopeType('AllExistingConnectedOrganizationSubjects');

requestorSettings.setAcceptRequests(true);

requestorSettings.setAllowedRequestors([]);


request_body.setRequestorSettings($requestorSettings);
requestApprovalSettings = ApprovalSettings();
requestApprovalSettings.setIsApprovalRequired(true);

requestApprovalSettings.setIsApprovalRequiredForExtension(false);

requestApprovalSettings.setIsRequestorJustificationRequired(true);

requestApprovalSettings.setApprovalMode('SingleStage');

approvalStagesApprovalStage1 = ApprovalStage();
approvalStagesApprovalStage1.setApprovalStageTimeOutInDays(14);

approvalStagesApprovalStage1.setIsApproverJustificationRequired(true);

approvalStagesApprovalStage1.setIsEscalationEnabled(false);

approvalStagesApprovalStage1.setEscalationTimeInMinutes(11520);

primaryApproversUserSet1 = UserSet();
primaryApproversUserSet1.set@odatatype('#microsoft.graph.groupMembers');

primaryApproversUserSet1.setIsBackup(true);

additionalData = [
'id' => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.setAdditionalData(additionalData);



primaryApproversArray []= primaryApproversUserSet1;
primaryApproversUserSet2 = UserSet();
primaryApproversUserSet2.set@odatatype('#microsoft.graph.externalSponsors');

primaryApproversUserSet2.setIsBackup(false);


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.setPrimaryApprovers(primaryApproversArray);



approvalStagesArray []= approvalStagesApprovalStage1;
requestApprovalSettings.setApprovalStages(approvalStagesArray);



request_body.setRequestApprovalSettings($requestApprovalSettings);
questionsAccessPackageQuestion1 = AccessPackageQuestion();
questionsAccessPackageQuestion1.setIsRequired(false);

questionsAccessPackageQuestion1Text = AccessPackageLocalizedContent();
questionsAccessPackageQuestion1Text.setDefaultText('what state are you from?');

localizedTextsAccessPackageLocalizedText1 = AccessPackageLocalizedText();
localizedTextsAccessPackageLocalizedText1.setText('¿De qué estado eres?');

localizedTextsAccessPackageLocalizedText1.setLanguageCode('es');


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion1Text.setLocalizedTexts(localizedTextsArray);



questionsAccessPackageQuestion1.setText($questionsAccessPackageQuestion1Text);
questionsAccessPackageQuestion1.set@odatatype('#microsoft.graph.accessPackageMultipleChoiceQuestion');

additionalData = [
'choices' => choices1 = ();
choices1.setActualValue('AZ');

choices1DisplayValue = DisplayValue();
localizedTexts1 = ();
localizedTexts1.setText('Arizona');

localizedTexts1.setLanguageCode('es');


localizedTextsArray []= localizedTexts1;
choices1DisplayValue.setLocalizedTexts(localizedTextsArray);



choices1.setDisplayValue($choices1DisplayValue);

choicesArray []= choices1;
choices2 = ();
choices2.setActualValue('CA');

choices2DisplayValue = DisplayValue();
localizedTexts1 = ();
localizedTexts1.setText('California');

localizedTexts1.setLanguageCode('es');


localizedTextsArray []= localizedTexts1;
choices2DisplayValue.setLocalizedTexts(localizedTextsArray);



choices2.setDisplayValue($choices2DisplayValue);

choicesArray []= choices2;
questionsAccessPackageQuestion1.setChoices(choicesArray);


'allowsMultipleSelection' => false,
];
questionsAccessPackageQuestion1.setAdditionalData(additionalData);



questionsArray []= questionsAccessPackageQuestion1;
questionsAccessPackageQuestion2 = AccessPackageQuestion();
questionsAccessPackageQuestion2.setIsRequired(false);

questionsAccessPackageQuestion2Text = AccessPackageLocalizedContent();
questionsAccessPackageQuestion2Text.setDefaultText('Who is your manager?');

localizedTextsAccessPackageLocalizedText1 = AccessPackageLocalizedText();
localizedTextsAccessPackageLocalizedText1.setText('por qué necesita acceso a este paquete');

localizedTextsAccessPackageLocalizedText1.setLanguageCode('es');


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion2Text.setLocalizedTexts(localizedTextsArray);



questionsAccessPackageQuestion2.setText($questionsAccessPackageQuestion2Text);
questionsAccessPackageQuestion2.set@odatatype('#microsoft.graph.accessPackageTextInputQuestion');

additionalData = [
'isSingleLineQuestion' => false,
];
questionsAccessPackageQuestion2.setAdditionalData(additionalData);



questionsArray []= questionsAccessPackageQuestion2;
request_body.setQuestions(questionsArray);




result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPoliciesById('accessPackageAssignmentPolicy-id').put(request_body);


```
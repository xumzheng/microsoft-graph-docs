---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.accessPackageId = 'b2eba9a1-b357-42ee-83a8-336522ed6cbf'

request_body.displayName = 'Users from connected organizations can request'

request_body.description = 'Allow users from configured connected organizations to request and be approved by their sponsors'

request_body.can_extend = False

request_body.duration_in_days = 365

request_body.expirationDateTime=null

requestor_settings = RequestorSettings()
requestorSettings.scopeType = 'AllExistingConnectedOrganizationSubjects'

requestorSettings.accept_requests = True


request_body.requestor_settings = requestorSettings
request_approval_settings = ApprovalSettings()
requestApprovalSettings.is_approval_required = True

requestApprovalSettings.is_approval_required_for_extension = False

requestApprovalSettings.is_requestor_justification_required = True

requestApprovalSettings.approvalMode = 'SingleStage'

approval_stages_approval_stage1 = ApprovalStage()
approvalStagesApprovalStage1.approval_stage_time_out_in_days = 14

approvalStagesApprovalStage1.is_approver_justification_required = True

approvalStagesApprovalStage1.is_escalation_enabled = False

approvalStagesApprovalStage1.escalation_time_in_minutes = 11520

primary_approvers_user_set1 = UserSet()
primaryApproversUserSet1.@odatatype = '#microsoft.graph.groupMembers'

primaryApproversUserSet1.is_backup = True

additionalData = [
'id' => 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf', 
'description' => 'group for users from connected organizations which have no external sponsor', 
];
primaryApproversUserSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversUserSet1;
primary_approvers_user_set2 = UserSet()
primaryApproversUserSet2.@odatatype = '#microsoft.graph.externalSponsors'

primaryApproversUserSet2.is_backup = False


primaryApproversArray []= primaryApproversUserSet2;
approvalStagesApprovalStage1.primaryapprovers(primaryApproversArray)



approvalStagesArray []= approvalStagesApprovalStage1;
requestApprovalSettings.approvalstages(approvalStagesArray)



request_body.request_approval_settings = requestApprovalSettings
questions_access_package_question1 = AccessPackageQuestion()
questionsAccessPackageQuestion1.is_required = False

questions_access_package_question1_text = AccessPackageLocalizedContent()
questionsAccessPackageQuestion1Text.defaultText = 'what state are you from?'

localized_texts_access_package_localized_text1 = AccessPackageLocalizedText()
localizedTextsAccessPackageLocalizedText1.text = '¿De qué estado eres?'

localizedTextsAccessPackageLocalizedText1.languageCode = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion1Text.localizedtexts(localizedTextsArray)



questionsAccessPackageQuestion1.text = questionsAccessPackageQuestion1Text
questionsAccessPackageQuestion1.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

additionalData = [
'choices' => choices1 = ()
choices1.actualValue = 'AZ'

choices1_display_value = DisplayValue()
localized_texts1 = ()
localizedTexts1.text = 'Arizona'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices1DisplayValue.localizedtexts(localizedTextsArray)



choices1.display_value = choices1DisplayValue

choicesArray []= choices1;
choices2 = ()
choices2.actualValue = 'CA'

choices2_display_value = DisplayValue()
localized_texts1 = ()
localizedTexts1.text = 'California'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices2DisplayValue.localizedtexts(localizedTextsArray)



choices2.display_value = choices2DisplayValue

choicesArray []= choices2;
choices3 = ()
choices3.actualValue = 'OH'

choices3_display_value = DisplayValue()
localized_texts1 = ()
localizedTexts1.text = 'Ohio'

localizedTexts1.languageCode = 'es'


localizedTextsArray []= localizedTexts1;
choices3DisplayValue.localizedtexts(localizedTextsArray)



choices3.display_value = choices3DisplayValue

choicesArray []= choices3;
questionsAccessPackageQuestion1.choices(choicesArray)


'allowsMultipleSelection' => false,
];
questionsAccessPackageQuestion1.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion1;
questions_access_package_question2 = AccessPackageQuestion()
questionsAccessPackageQuestion2.is_required = False

questions_access_package_question2_text = AccessPackageLocalizedContent()
questionsAccessPackageQuestion2Text.defaultText = 'Who is your manager?'

localized_texts_access_package_localized_text1 = AccessPackageLocalizedText()
localizedTextsAccessPackageLocalizedText1.text = 'por qué necesita acceso a este paquete'

localizedTextsAccessPackageLocalizedText1.languageCode = 'es'


localizedTextsArray []= localizedTextsAccessPackageLocalizedText1;
questionsAccessPackageQuestion2Text.localizedtexts(localizedTextsArray)



questionsAccessPackageQuestion2.text = questionsAccessPackageQuestion2Text
questionsAccessPackageQuestion2.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

additionalData = [
'isSingleLineQuestion' => false,
];
questionsAccessPackageQuestion2.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)





result = await client.identityGovernance.entitlementManagement.accessPackageAssignmentPolicies.post(request_body = request_body)


```
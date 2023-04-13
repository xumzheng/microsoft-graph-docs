---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessPackageAssignmentPolicy()
request_body.displayName = 'A Policy With Questions'

request_body.description = ''

request_body.AllowedTargetScope(AllowedTargetScope('allmemberusers'))

expiration = ExpirationPattern()
expiration.Type(ExpirationPatternType('noexpiration'))


request_body.expiration = expiration
requestor_settings = AccessPackageAssignmentRequestorSettings()
requestorSettings.enable_targets_to_self_add_access = True

requestorSettings.enable_targets_to_self_update_access = True

requestorSettings.enable_targets_to_self_remove_access = True


request_body.requestor_settings = requestorSettings
request_approval_settings = AccessPackageAssignmentApprovalSettings()
requestApprovalSettings.is_approval_required_for_add = True

requestApprovalSettings.is_approval_required_for_update = True

stages_access_package_approval_stage1 = AccessPackageApprovalStage()
stagesAccessPackageApprovalStage1.durationbeforeautomaticdenial =  \DateInterval('P7D')

stagesAccessPackageApprovalStage1.is_approver_justification_required = False

stagesAccessPackageApprovalStage1.is_escalation_enabled = False

stagesAccessPackageApprovalStage1.FallbackPrimaryApprovers([])

stagesAccessPackageApprovalStage1.EscalationApprovers([])

stagesAccessPackageApprovalStage1.FallbackEscalationApprovers([])

primary_approvers_subject_set1 = SubjectSet()
primaryApproversSubjectSet1.@odatatype = '#microsoft.graph.singleUser'

additionalData = [
'userId' => '08a551cb-575a-4343-b914-f6e42798bd20', 
];
primaryApproversSubjectSet1.additionaldata(additionalData)



primaryApproversArray []= primaryApproversSubjectSet1;
stagesAccessPackageApprovalStage1.primaryapprovers(primaryApproversArray)



stagesArray []= stagesAccessPackageApprovalStage1;
requestApprovalSettings.stages(stagesArray)



request_body.request_approval_settings = requestApprovalSettings
questions_access_package_question1 = AccessPackageQuestion()
questionsAccessPackageQuestion1.@odatatype = '#microsoft.graph.accessPackageMultipleChoiceQuestion'

questionsAccessPackageQuestion1.sequence = 1

questionsAccessPackageQuestion1.is_required = True

questionsAccessPackageQuestion1.is_answer_editable = True

questionsAccessPackageQuestion1.text = 'What country are you working from?'

additionalData = [
'isMultipleSelectionAllowed' => 'false', 
'choices' => choices1 = ()
choices1.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices1.actualValue = 'KE'

choices1.text = 'Kenya'


choicesArray []= choices1;
choices2 = ()
choices2.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices2.actualValue = 'US'

choices2.text = 'United States'


choicesArray []= choices2;
choices3 = ()
choices3.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices3.actualValue = 'GY'

choices3.text = 'Guyana'


choicesArray []= choices3;
choices4 = ()
choices4.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices4.actualValue = 'BD'

choices4.text = 'Bangladesh'


choicesArray []= choices4;
choices5 = ()
choices5.@odatatype = 'microsoft.graph.accessPackageAnswerChoice'

choices5.actualValue = 'JP'

choices5.text = 'Japan'


choicesArray []= choices5;
questionsAccessPackageQuestion1.choices(choicesArray)


];
questionsAccessPackageQuestion1.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion1;
questions_access_package_question2 = AccessPackageQuestion()
questionsAccessPackageQuestion2.@odatatype = '#microsoft.graph.accessPackageTextInputQuestion'

questionsAccessPackageQuestion2.sequence = 2

questionsAccessPackageQuestion2.is_required = True

questionsAccessPackageQuestion2.is_answer_editable = True

questionsAccessPackageQuestion2.text = 'What do you do for work?'

localizations_access_package_localized_text1 = AccessPackageLocalizedText()
localizationsAccessPackageLocalizedText1.languageCode = 'fr-CA'

localizationsAccessPackageLocalizedText1.text = 'Que fais-tu comme travail?'


localizationsArray []= localizationsAccessPackageLocalizedText1;
questionsAccessPackageQuestion2.localizations(localizationsArray)


additionalData = [
'isSingleLineQuestion' => 'false', 
'regexPattern' => '[a-zA-Z]+[a-zA-Z\s]*', 
];
questionsAccessPackageQuestion2.additionaldata(additionalData)



questionsArray []= questionsAccessPackageQuestion2;
request_body.questions(questionsArray)


access_package = AccessPackage()
accessPackage.id = '977c7ff4-ef8f-4910-9d31-49048ddf3120'


request_body.access_package = accessPackage



result = await client.identityGovernance.entitlementManagement.assignmentPolicies.post(request_body = request_body)


```
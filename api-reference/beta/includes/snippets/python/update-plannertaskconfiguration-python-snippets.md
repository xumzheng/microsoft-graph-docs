---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PlannerTaskConfiguration()
request_body.set@odatatype('#microsoft.graph.plannerTaskConfiguration')

editPolicy = PlannerTaskPolicy()
rulesPlannerTaskRoleBasedRule1 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule1.setDefaultRule('block')

rulesPlannerTaskRoleBasedRule1Role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule1Role.set@odatatype('#microsoft.graph.plannerRelationshipBasedUserType')

rulesPlannerTaskRoleBasedRule1Role.setRoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'defaultRules', 
];
rulesPlannerTaskRoleBasedRule1Role.setAdditionalData(additionalData)



rulesPlannerTaskRoleBasedRule1.setRole($rulesPlannerTaskRoleBasedRule1Role)
rulesPlannerTaskRoleBasedRule1PropertyRule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule1PropertyRule.setPercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule1PropertyRule.setRuleKind(PlannerRuleKind('taskrule'))

rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.setDefaultRules(['addSelf', ])

rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.setOverrides([])


rulesPlannerTaskRoleBasedRule1PropertyRule.setAssignments($rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments)

rulesPlannerTaskRoleBasedRule1.setPropertyRule($rulesPlannerTaskRoleBasedRule1PropertyRule)

rulesArray []= rulesPlannerTaskRoleBasedRule1;
rulesPlannerTaskRoleBasedRule2 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule2.setDefaultRule('block')

rulesPlannerTaskRoleBasedRule2Role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule2Role.set@odatatype('#microsoft.graph.plannerRelationshipBasedUserType')

rulesPlannerTaskRoleBasedRule2Role.setRoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'taskAssignees', 
];
rulesPlannerTaskRoleBasedRule2Role.setAdditionalData(additionalData)



rulesPlannerTaskRoleBasedRule2.setRole($rulesPlannerTaskRoleBasedRule2Role)
rulesPlannerTaskRoleBasedRule2PropertyRule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule2PropertyRule.setStartDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.setDueDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.setPercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.setOrder(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.setRuleKind(PlannerRuleKind('taskrule'))

rulesPlannerTaskRoleBasedRule2PropertyRuleReferences = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.setDefaultRules(['allow', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.setName('userCreated')

overridesPlannerRuleOverride1.setRules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.setName('applicationCreated')

overridesPlannerRuleOverride2.setRules(['block', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.setOverrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.setReferences($rulesPlannerTaskRoleBasedRule2PropertyRuleReferences)
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.setDefaultRules(['allow', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.setName('userCreated')

overridesPlannerRuleOverride1.setRules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.setName('applicationCreated')

overridesPlannerRuleOverride2.setRules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.setOverrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.setCheckLists($rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists)
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.setDefaultRules(['block', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.setName('userCreated')

overridesPlannerRuleOverride1.setRules(['removeSelf', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.setName('applicationCreated')

overridesPlannerRuleOverride2.setRules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.setOverrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.setAssignments($rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments)
rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.setDefaultRules(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.setOverrides([])


rulesPlannerTaskRoleBasedRule2PropertyRule.setAppliedCategories($rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories)

rulesPlannerTaskRoleBasedRule2.setPropertyRule($rulesPlannerTaskRoleBasedRule2PropertyRule)

rulesArray []= rulesPlannerTaskRoleBasedRule2;
editPolicy.setRules(rulesArray)



request_body.setEditPolicy($editPolicy)


result = await client.solutions.businessScenariosById('businessScenario-id').planner.taskConfiguration.patch(request_body)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```cli

mgc groups list --filter mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT(groupTypes/any(s:s%20eq%20'Unified'))%20and%20membershipRuleProcessingState%20eq%20'On' --count true --select id,membershipRule,membershipRuleProcessingState --consistency-level eventual

```
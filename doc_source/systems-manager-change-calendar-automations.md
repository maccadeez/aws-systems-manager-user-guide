# Adding Change Calendar dependencies to Automation runbooks<a name="systems-manager-change-calendar-automations"></a>

To make Automation actions adhere to Change Calendar, a capability of AWS Systems Manager, add a step in an Automation runbook that uses the [`aws:assertAwsResourceProperty`](automation-action-assertAwsResourceProperty.md) action\. Configure the action to run `GetCalendarState` to verify that a specified calendar entry is in the state that you want \(`OPEN` or `CLOSED`\)\. The Automation runbook is only allowed to continue to the next step if the calendar state is `OPEN`\. The following is a YAML\-based sample excerpt of an Automation runbook that can't advance to the next step, `LaunchInstance`, unless the calendar state matches `OPEN`, the state specified in `DesiredValues`\.

The following is an example\.

```
mainSteps:
  - name: MyCheckCalendarStateStep
    action: 'aws:assertAwsResourceProperty'
    inputs:
      Service: ssm
      Api: GetCalendarState
      CalendarNames: ["arn:aws:ssm:us-east-2:123456789012:document/SaleDays"]
      PropertySelector: '$.State'
      DesiredValues:
      - OPEN
    description: "Use GetCalendarState to determine whether a calendar is open or closed."
    nextStep: LaunchInstance
  - name: LaunchInstance
    action: 'aws:executeScript'
    inputs:
      Runtime: python3.6 
...
```
PR needs reviewer checklist completed by a Developer reviewer and QE reviewer prior to merge

Developer reviewer:
- [ ] Code looks sound, good architectural decisions, no [code smells](https://www.codegrip.tech/productivity/everything-you-need-to-know-about-code-smells/)
- [ ] There is a Jira issue associated (note that "No-Issue" should be rarely used)
- [ ] There are unit & functional tests in PR, and they fully cover necessary test scenarios... or code update does not need unit or functional tests, i.e. a dependency update, etc.

QE reviewer:
- [ ] There are unit & functional tests in PR, and they fully cover necessary test scenarios... or code update does not need unit or functional tests, i.e. a dependency update, etc.
- [ ] PR meets applicable Acceptance Criteria for associated Jira issue
- [ ] An IQE test is not needed... or an [IQE test is needed](https://docs.engineering.redhat.com/display/AUTOHUB/Other+Team+Processes#OtherTeamProcesses-IQETests), and it is written and merged, and CI passes after `/retest` comment. Note: If IQE test is needed, mark PR as "Request Changes" until IQE test is written and merged.

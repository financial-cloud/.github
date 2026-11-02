<!--
Sections marked [monday] are synced to the linked ticket on the Monday Tasks board
when the PR is opened and every time this description is edited.
Keep the "## " headings exactly as they are - they are how the sync finds each section.
Write N/A in a [monday] section that doesn't apply; it will be left empty on the ticket.
-->

## Monday ticket

<!-- Required. Paste the Monday item link or its Task ID, e.g.
https://fcloud-company.monday.com/boards/5097440571/pulses/3306069647  or  3306069647 -->


## Summary

<!-- [monday: posted as an update on the ticket] Why are you making this pull request? e.g.
- this PR fixes the sort not being applied when using the query
- a bug causes the SDK to have unhandled promise rejections, this PR updates `section` to correctly handle errors
- this PR refactors `section` to make it more maintainable -->


## All changes

<!-- [monday: posted as an update on the ticket] -->
- **Added:**
- **Updated:**
- **Removed:**
- **Refactored:**

## Breaking changes

<!-- [monday: posted as an update on the ticket] Remove or write N/A if there are none.
Why were the breaking changes needed? Which teams / services are affected? -->


- [ ] Updated tests to reflect breaking changes
- [ ] Informed relevant teams of the changes

## PR check list

- [ ] Version bump
- [ ] Updated / Added tests
- [ ] Updated postman with new/updated routes
- [ ] Documentation
- [ ] Deployment sections below filled in (or marked N/A)

## Database changes

<!-- [monday: Database changes] System tables (new or updated rows and their values) and new collections (name and seed data), e.g.
System tables: add `FCCORE_preferredContactTime` to `systemtables` (level: customer, _collection: crm)
New collections: `callflowreasons` - seed with the default call flow reasons -->


## Index changes

<!-- [monday: Index changes] Collection, fields, unique/sparse/TTL options, e.g.
`crm` - { FCCID: 1, property: 1 }
`chargeCodes` - { code: 1 } (unique) -->


## Scripts

<!-- [monday: Scripts] Migration / one-off scripts that must be run, where they live and when to run them -->


## Configuration changes

<!-- [monday: Configuration changes] Feature flags, environment variables, settings, e.g.
be-communications - new env var `SMS_PROVIDER_TIMEOUT_MS` in all environments -->


## Miscellaneous deployment notes

<!-- [monday: Miscellaneous deployment notes] Anything else needed to deploy: ordering, downtime, dependencies on other PRs -->


## Test notes

<!-- [monday: Test notes] How this was tested and what QA should check -->


<!--
Sections marked [monday] are synced to the linked ticket whenever the PR is opened or edited. 
Keep the headings exactly as they are, write N/A in any [monday] section that doesn’t apply, and note that the examples are hidden in comments.
Put the Task ID in the commits, branch name and PR title so the PR also shows in the ticket’s Git UI.
-->

## Monday ticket

<!-- Required. Paste the full Monday ticket link.

#### Example

```
https://fcloud-company.monday.com/boards/5097440571/pulses/3306069647
```
-->


## Summary

<!-- [monday: PR summary] Why are you making this pull request?

#### Examples

```
this PR fixes the sort not being applied when using the query
```
-->


## All changes

- **Added:**
- **Updated:**
- **Removed:**
- **Refactored:**

<!--
#### Example

```
- **Added:** `GET /flow/contact-time` route for the preferred contact time options
- **Updated:** `crm` service saves `preferredContactTime` on the customer
- **Removed:** unused `legacyContactTime` helper
- **Refactored:** moved contact time validation into `validators/contact.ts`
```
-->

## Breaking changes

<!-- Remove or write N/A if there are none.
Why were the breaking changes needed? Which teams / services are affected?

#### Example

```
`GET /customer/profile` now returns `contactTime` as an object instead of a string.
```
-->

## PR check list

- [ ] Version bump
- [ ] Updated / Added tests
- [ ] Updated postman with new/updated routes
- [ ] Documentation
- [ ] Deployment sections below filled in (or marked N/A)

## Database changes

<!-- [monday: Database changes] System tables (new or updated rows and their values) and new collections.

#### Example

```
System tables: add `FCCORE_preferredContactTime` to `systemtables` (level: customer, _collection: crm)

New collection: `callflowreasons` 
```
-->


## Index changes

<!-- [monday: Index changes] Collection, fields, unique/sparse/TTL options.

#### Example

```
`crm` - { FCCID: 1, property: 1 }
```
-->


## Scripts

<!-- [monday: Scripts] Migration / one-off scripts that must be run and when to run them.
Link to the script in a GitHub repository, not a file on your machine.

#### Example

```
https://github.com/financial-cloud/fc-migrations/blob/main/migrations/backfill-preferred-contact-time.ts - run once on each environment before deploy
```
-->


## Configuration changes

<!-- [monday: Configuration changes] Feature flags, environment variables, settings.

#### Example

```
be-communications - new env var `SMS_PROVIDER_TIMEOUT_MS` in all environments
fe-customer-portal - enviroment `preferredContactTime` must be added to each customer
```
-->


## Miscellaneous deployment notes

<!-- [monday: Miscellaneous deployment notes] Anything else needed to deploy: ordering, downtime, dependencies on other PRs.

#### Example

```
Deploy after financial-cloud/helpdesk#693. No downtime expected.
```
-->


## Test notes

<!-- [monday: Test notes] How this was tested and what QA should check.

#### Example

```
QA: open the profile page, pick a preferred contact time, save, and check it's still set after a refresh.
```
-->


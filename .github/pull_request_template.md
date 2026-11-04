<!--
Sections marked [monday] are added to the matching field on the linked Monday ticket
when the PR is opened and every time this description is edited. Each PR's text goes
under its own "[repo #pr-number]" heading, so other PRs on the same ticket are kept.
Software versions is filled automatically from package.json.
Keep the "## " headings exactly as they are - they are how the sync finds each section.
Write N/A in a [monday] section that doesn't apply.
The examples are inside comments like this one, so they don't show on the PR or in Monday.
Put the Task ID in the branch name (e.g. fix/3305431211-uploads-lambda) or PR title so the
PR also shows in the monday ticket's Git UI.
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

```
a bug causes the SDK to have unhandled promise rejections, this PR updates `section` to correctly handle errors
```

```
this PR refactors `section` to make it more maintainable
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
fe-customer-portal and fe-online-helpdesk need the matching release.
```
-->


- [ ] Updated tests to reflect breaking changes
- [ ] Informed relevant teams of the changes

## PR check list

- [ ] Version bump
- [ ] Updated / Added tests
- [ ] Updated postman with new/updated routes
- [ ] Documentation
- [ ] Deployment sections below filled in (or marked N/A)

## Database changes

<!-- [monday: Database changes] System tables (new or updated rows and their values) and new collections (name and seed data).

#### Example

```
System tables: add `FCCORE_preferredContactTime` to `systemtables` (level: customer, _collection: crm)
System tables: update `FCCORE_preferredContactTime` in `systemtables` - change `level` from customer to client
New collections: `callflowreasons` - seed with the default call flow reasons
```
-->


## Index changes

<!-- [monday: Index changes] Collection, fields, unique/sparse/TTL options.

#### Example

```
`crm` - { FCCID: 1, property: 1 }
`chargeCodes` - { code: 1 } (unique)
```
-->


## Scripts

<!-- [monday: Scripts] Migration / one-off scripts that must be run and when to run them.
Link to the script in a GitHub repository, not a file on your machine.

#### Example

```
https://github.com/financial-cloud/fc-migrations/blob/main/migrations/backfill-preferred-contact-time.ts - run once on each environment after deploy
```
-->


## Configuration changes

<!-- [monday: Configuration changes] Feature flags, environment variables, settings.

#### Example

```
be-communications - new env var `SMS_PROVIDER_TIMEOUT_MS` in all environments
helpdesk - feature flag `preferredContactTime` on for staging only
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
Tested locally against staging data.
QA: open the profile page, pick a preferred contact time, save, and check it's still set after a refresh.
```
-->


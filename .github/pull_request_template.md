# Motivation

why are you making this pull request? 

#### Examples

```
This Pr fixes bug https://fcloud-company.monday.com/boards/1315295767/pulses/1316778205

```

```
a bug causes the SDK to have unhandled promise rejections, this PR updates `section` to correctly handle errors
```

```
this PR refactors `section` to make it more maintainable
```

# PR check list

- [ ] version bump
- [ ] Updated / Added tests
- [ ] Updated postman with new/updated routes
- [ ] Documentation
- [ ] Deployment requirements listed below (or marked N/A)


# Deployment Requirements

List everything that must exist or be configured in an environment for this PR to work. Mark a line N/A if it doesn't apply, so reviewers know it was considered.

- **Indexes:** (collection, fields, unique/sparse/TTL options)
- **System tables:** (new or updated rows/records and their values)
- **New collections:** (name, and any seed data required)
- **Other system configuration:** (feature flags, environment variables, settings etc.)

#### Example

```
Indexes: `crm` - { FCCID: 1, property: 1 }
         `chargeCodes` - { code: 1 } (unique)
System tables: add `FCCORE_preferredContactTime` to `systemtables` (level: customer, _collection: crm)
New collections: `callflowreasons` - seed with the default call flow reasons
Other system configuration: be-communications - new env var `SMS_PROVIDER_TIMEOUT_MS` in all environments
```


# Breaking Changes

you can remove this section if there are none

Why were the breaking changes needed?

## Breaking change check test

- [ ] Updated tests to reflect breaking changes
- [ ] Informed relevant teams of the changes


### All Changes

- **Added:**
- **Updated:** 
- **Removed:** 
- **Refactored:** 
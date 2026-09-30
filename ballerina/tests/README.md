# Running Tests

## Prerequisites

The tests run against a mock server by default, so no credentials are needed.

To run them against the live Xero Projects API, set:

```bash
export IS_LIVE_SERVER=true
export XERO_ACCESS_TOKEN=<access-token>
export XERO_TENANT_ID=<xero-tenant-id>
```

Mutating tests are skipped against the live server, and the read tests need the fixed project, task and time entry IDs to exist in the organisation.

## Test scenarios

The suite covers all 16 operations of the client: listing, creating, retrieving, updating, closing and deleting projects, tasks and time entries, and listing project users.

## Running the tests

```bash
bal test
```

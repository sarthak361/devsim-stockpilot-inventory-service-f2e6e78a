# StockPilot Inventory Service

Business brief: A warehouse oversells products during simultaneous orders. Implement catalog pagination, stock reservations, atomic inventory changes, authorization and audit logs. Milestones: 1. Validated inventory API; 2. Concurrency-safe reservations; 3. Integration and performance tests. Start a Spring Boot service with PostgreSQL. Deliver a documented repository with reproducible tests. No pre-existing repository is bundled.

## DevSim ticket workflow
Clone this repository. Create a feature branch using the exact ticket key below. Push changes and open a PR against the default branch. DevSim links PRs authored by your connected GitHub account automatically.

### STO-F75A-103: Handle missing resources
Branch: `feature/sto-f75a-103`

- Return a clear not-found result for unknown IDs.
- Preserve the successful retrieval behavior.
- Test existing and missing IDs.

### STO-F75A-102: Validate resource creation
Branch: `feature/sto-f75a-102`

- Reject blank required fields with a clear error.
- Create a record for valid input.
- Add tests for valid and invalid input.

### STO-F75A-101: Build the first resource listing
Branch: `feature/sto-f75a-101`

- Return the resource list with a predictable data shape.
- Handle an empty dataset without crashing.
- Add tests for normal and empty results.

### STO-F75A-105: Add an update workflow
Branch: `feature/sto-f75a-105`

- Update editable fields for an existing ID.
- Validate required fields on update.
- Add tests for valid, invalid and missing resources.

### STO-F75A-106: Document the core workflow
Branch: `feature/sto-f75a-106`

- Include setup instructions and example inputs in the README.
- Explain errors and expected results.
- Include a repeatable smoke-test procedure.

### STO-F75A-104: Add status filtering
Branch: `feature/sto-f75a-104`

- Filter records by active status.
- Reject unsupported filter values.
- Test matching, non-matching and empty results.


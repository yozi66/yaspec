# Tasks: Asset Tracking Application

**Input**: Design documents from `/specs/main/`
**Prerequisites**: plan.md, research.md, data-model.md, contracts/

## Phase 3.1: Setup
- [ ] T001 Create `frontend` and `backend` project structure
- [ ] T002 [P] Initialize Node.js project in `backend` and install dependencies (electron, typescript, sqlite3)
- [ ] T003 [P] Initialize React project in `frontend` with TypeScript and install dependencies (react, mantine)
- [ ] T004 [P] Configure ESLint and Prettier for both `frontend` and `backend`
- [ ] T005 Set up the basic Electron application shell in `backend/src/main.ts`

## Phase 3.2: Tests First (TDD) ⚠️ MUST COMPLETE BEFORE 3.3
**CRITICAL: These tests MUST be written and MUST FAIL before ANY implementation**
- [ ] T006 [P] Contract test for Owner IPC in `backend/tests/contract/owner.test.ts`
- [ ] T007 [P] Contract test for Bank IPC in `backend/tests/contract/bank.test.ts`
- [ ] T008 [P] Contract test for Account IPC in `backend/tests/contract/account.test.ts`
- [ ] T009 [P] Contract test for Asset IPC in `backend/tests/contract/asset.test.ts`
- [ ] T010 [P] Integration test for owner management flow in `backend/tests/integration/owner-flow.test.ts`
- [ ] T011 [P] Integration test for bank management flow in `backend/tests/integration/bank-flow.test.ts`
- [ ] T012 [P] Integration test for account management flow in `backend/tests/integration/account-flow.test.ts`
- [ ] T013 [P] Integration test for asset management flow in `backend/tests/integration/asset-flow.test.ts`

## Phase 3.3: Core Implementation (ONLY after tests are failing)
- [ ] T014 [P] Create data models for Owner, Bank, Account, Asset in `backend/src/models.ts`
- [ ] T015 [P] Implement OwnerService in `backend/src/services/owner-service.ts`
- [ ] T016 [P] Implement BankService in `backend/src/services/bank-service.ts`
- [ ] T017 Implement AccountService in `backend/src/services/account-service.ts` (depends on OwnerService, BankService)
- [ ] T018 Implement AssetService in `backend/src/services/asset-service.ts` (depends on AccountService)
- [ ] T019 Implement IPC handlers for all entities in `backend/src/ipc-handlers.ts`
- [ ] T020 [P] Create Owner management UI components in `frontend/src/components/owners`
- [ ] T021 [P] Create Bank management UI components in `frontend/src/components/banks`
- [ ] T022 [P] Create Account management UI components in `frontend/src/components/accounts`
- [ ] T023 [P] Create Asset management UI components in `frontend/src/components/assets`
- [ ] T024 Create Dashboard page in `frontend/src/pages/Dashboard.tsx`

## Phase 3.4: Integration
- [ ] T025 Implement database initialization and connection in `backend/src/database.ts`
- [ ] T026 Integrate services with the database
- [ ] T027 Set up IPC communication between `frontend` and `backend`

## Phase 3.5: Polish
- [ ] T028 [P] Write unit tests for UI components
- [ ] T029 [P] Write unit tests for utility functions
- [ ] T030 Perform performance testing and optimization based on `research.md`
- [ ] T031 Implement password protection for the database file
- [ ] T032 Finalize documentation and update `README.md`

## Dependencies
- Setup (T001-T005) before all other tasks.
- Tests (T006-T013) before Core Implementation (T014-T024).
- T014 (Models) before T015-T018 (Services).
- T015, T016 before T017.
- T017 before T018.
- Core Implementation (T014-T024) before Integration (T025-T027).
- Integration (T025-T027) before Polish (T028-T032).

## Parallel Example
```
# Launch contract tests together:
Task: "Contract test for Owner IPC in backend/tests/contract/owner.test.ts"
Task: "Contract test for Bank IPC in backend/tests/contract/bank.test.ts"
Task: "Contract test for Account IPC in backend/tests/contract/account.test.ts"
Task: "Contract test for Asset IPC in backend/tests/contract/asset.test.ts"
```

# Tasks: Asset Tracking Application

**Input**: Design documents from `/specs/main/`
**Prerequisites**: plan.md, research.md, data-model.md, contracts/

## Phase 3.1: Setup
- [ ] T001 Clone the `electron-vite-react` template
- [ ] T002 Install project dependencies
- [ ] T003 Configure linting and formatting tools

## Phase 3.2: Tests First (TDD) ⚠️ MUST COMPLETE BEFORE 3.3
**CRITICAL: These tests MUST be written and MUST FAIL before ANY implementation**
- [ ] T004 [P] Contract test for Owner IPC in `src/main/tests/contract/owner.test.ts`
- [ ] T005 [P] Contract test for Bank IPC in `src/main/tests/contract/bank.test.ts`
- [ ] T006 [P] Contract test for Account IPC in `src/main/tests/contract/account.test.ts`
- [ ] T007 [P] Contract test for Asset IPC in `src/main/tests/contract/asset.test.ts`
- [ ] T008 [P] Integration test for owner management flow in `src/main/tests/integration/owner-flow.test.ts`
- [ ] T009 [P] Integration test for bank management flow in `src/main/tests/integration/bank-flow.test.ts`
- [ ] T010 [P] Integration test for account management flow in `src/main/tests/integration/account-flow.test.ts`
- [ ] T011 [P] Integration test for asset management flow in `src/main/tests/integration/asset-flow.test.ts`

## Phase 3.3: Core Implementation (ONLY after tests are failing)
- [ ] T012 [P] Create data models for Owner, Bank, Account, Asset in `src/main/models.ts`
- [ ] T013 [P] Implement OwnerService in `src/main/services/owner-service.ts`
- [ ] T014 [P] Implement BankService in `src/main/services/bank-service.ts`
- [ ] T015 Implement AccountService in `src/main/services/account-service.ts` (depends on OwnerService, BankService)
- [ ] T016 Implement AssetService in `src/main/services/asset-service.ts` (depends on AccountService)
- [ ] T017 Implement IPC handlers for all entities in `src/main/ipc-handlers.ts`
- [ ] T018 [P] Create Owner management UI components in `src/renderer/src/components/owners`
- [ ] T019 [P] Create Bank management UI components in `src/renderer/src/components/banks`
- [ ] T020 [P] Create Account management UI components in `src/renderer/src/components/accounts`
- [ ] T021 [P] Create Asset management UI components in `src/renderer/src/components/assets`
- [ ] T022 Create Dashboard page in `src/renderer/src/pages/Dashboard.tsx`

## Phase 3.4: Integration
- [ ] T023 Implement database initialization and connection in `src/main/database.ts`
- [ ] T024 Integrate services with the database
- [ ] T025 Set up IPC communication in `src/preload/index.ts`

## Phase 3.5: Polish
- [ ] T026 [P] Write unit tests for UI components
- [ ] T027 [P] Write unit tests for utility functions
- [ ] T028 Perform performance testing and optimization based on `research.md`
- [ ] T029 Implement password protection for the database file
- [ ] T030 Finalize documentation and update `README.md`

## Dependencies
- Setup (T001-T003) before all other tasks.
- Tests (T004-T011) before Core Implementation (T012-T022).
- T012 (Models) before T013-T016 (Services).
- T013, T014 before T015.
- T015 before T016.
- Core Implementation (T012-T022) before Integration (T023-T025).
- Integration (T023-T025) before Polish (T026-T030).
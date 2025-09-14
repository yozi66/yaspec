# Contract Tests

This document outlines the contract tests for the IPC channels.

## Owner Contracts

-   **`owners:get-all`**:
    -   Test that the backend returns an array of owners.
    -   Test that the array is empty if no owners exist.
-   **`owners:create`**:
    -   Test that a new owner is created with the correct name.
    -   Test that the created owner is returned.
-   **`owners:update`**:
    -   Test that an existing owner is updated with the correct name.
    -   Test that the updated owner is returned.
-   **`owners:delete`**:
    -   Test that an owner is deleted.
    -   Test that the backend does not throw an error if the owner does not exist.

## Bank Contracts

-   **`banks:get-all`**:
    -   Test that the backend returns an array of banks.
    -   Test that the array is empty if no banks exist.
-   **`banks:create`**:
    -   Test that a new bank is created with the correct name.
    -   Test that the created bank is returned.
-   **`banks:update`**:
    -   Test that an existing bank is updated with the correct name.
    -   Test that the updated bank is returned.
-   **`banks:delete`**:
    -   Test that a bank is deleted.
    -   Test that the backend does not throw an error if the bank does not exist.

## Account Contracts

-   **`accounts:get-all`**:
    -   Test that the backend returns an array of accounts.
    -   Test that the array is empty if no accounts exist.
-   **`accounts:create`**:
    -   Test that a new account is created with the correct data.
    -   Test that the created account is returned.
-   **`accounts:update`**:
    -   Test that an existing account is updated with the correct data.
    -   Test that the updated account is returned.
-   **`accounts:delete`**:
    -   Test that an account is deleted.
    -   Test that the backend does not throw an error if the account does not exist.

## Asset Contracts

-   **`assets:get-all`**:
    -   Test that the backend returns an array of assets.
    -   Test that the array is empty if no assets exist.
-   **`assets:create`**:
    -   Test that a new asset is created with the correct data.
    -   Test that the created asset is returned.
-   **`assets:update`**:
    -   Test that an existing asset is updated with the correct data.
    -   Test that the updated asset is returned.
-   **`assets:delete`**:
    -   Test that an asset is deleted.
    -   Test that the backend does not throw an error if the asset does not exist.

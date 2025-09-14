# Account IPC Contracts

-   **`accounts:get-all`**:
    -   Direction: Frontend -> Backend
    -   Payload: none
    -   Returns: `Account[]`
-   **`accounts:create`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Omit<Account, 'id'>`
    -   Returns: `Account`
-   **`accounts:update`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Account`
    -   Returns: `Account`
-   **`accounts:delete`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ id: string }`
    -   Returns: `void`

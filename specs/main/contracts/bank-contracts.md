# Bank IPC Contracts

-   **`banks:get-all`**:
    -   Direction: Frontend -> Backend
    -   Payload: none
    -   Returns: `Bank[]`
-   **`banks:create`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ name: string }`
    -   Returns: `Bank`
-   **`banks:update`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Bank`
    -   Returns: `Bank`
-   **`banks:delete`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ id: string }`
    -   Returns: `void`

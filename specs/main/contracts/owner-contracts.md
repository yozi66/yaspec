# Owner IPC Contracts

-   **`owners:get-all`**:
    -   Direction: Frontend -> Backend
    -   Payload: none
    -   Returns: `Owner[]`
-   **`owners:create`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ name: string }`
    -   Returns: `Owner`
-   **`owners:update`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Owner`
    -   Returns: `Owner`
-   **`owners:delete`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ id: string }`
    -   Returns: `void`

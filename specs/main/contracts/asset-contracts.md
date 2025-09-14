# Asset IPC Contracts

-   **`assets:get-all`**:
    -   Direction: Frontend -> Backend
    -   Payload: none
    -   Returns: `Asset[]`
-   **`assets:create`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Omit<Asset, 'id'>`
    -   Returns: `Asset`
-   **`assets:update`**:
    -   Direction: Frontend -> Backend
    -   Payload: `Asset`
    -   Returns: `Asset`
-   **`assets:delete`**:
    -   Direction: Frontend -> Backend
    -   Payload: `{ id: string }`
    -   Returns: `void`

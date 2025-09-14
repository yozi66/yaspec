# Data Model

This document defines the data entities for the asset tracking application.

## Owner

Represents a family member who owns assets.

-   `id`: string (unique identifier)
-   `name`: string (e.g., "John Doe")

## Bank

Represents a financial institution.

-   `id`: string (unique identifier)
-   `name`: string (e.g., "Big Bank Inc.")

## Account

Represents a bank account.

-   `id`: string (unique identifier)
-   `bankId`: string (foreign key to Bank)
-   `ownerId`: string (foreign key to Owner)
-   `name`: string (e.g., "Investment Account")
-   `type`: string (e.g., "general", "tbsz")
-   `tbszMaturityDate`: date (optional, for TBSZ accounts)

## Asset

Represents a financial asset.

-   `id`: string (unique identifier)
-   `accountId`: string (foreign key to Account)
-   `name`: string (e.g., "Apple Inc.")
-   `ticker`: string (e.g., "AAPL")
-   `type`: string (e.g., "stock", "bond", "etf")
-   `purchaseDate`: date
-   `purchasePrice`: number
-   `quantity`: number

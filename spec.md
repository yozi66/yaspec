**Application Type and Core Purpose:**

A full-stack web application to track financial assets like bonds, stocks, and ETFs for some users in a family. It will support multiple banks and accounts, including special Hungarian TBSZ accounts with their 5-year tax-benefit lifecycle.

**Key Technologies:**

*   **Frontend:** React with TypeScript, using Mantine for a modern, responsive user interface.
*   **Backend:** Node.js with Electron (TypeScript).
*   **Database:** I will use a simple file-based database (like SQLite or a JSON file) for the initial prototype to ensure a quick and easy setup. The database should be easy to copy or move to another computer. 

**Main Features and User Interaction:**
*   **Dashboard:** A central dashboard will provide an at-a-glance overview of your total portfolio value, asset allocation charts, and recent performance.
*   **Asset Management:** You will be able to add, edit, and delete your assets (stocks, bonds, ETFs), specifying the owner, bank, account, purchase date, price, and quantity.
*   **TBSZ Account Tracking:** A dedicated section will manage TBSZ accounts, tracking their 5-year maturity date and providing visual indicators for the remaining time.
*   **Single user desktop app:** The application will distinguish between assets belonging to the individual owners (family members), but there is no need for user management. The application and the database have an option to be protected by a password (and stored encoded). 

**Visual Design and UX:**
The application will feature a clean, modern, and intuitive design based on Mantine. The dashboard will serve as the main entry point, offering a comprehensive overview, while dedicated sections will allow for easy management of individual portfolios and TBSZ accounts.

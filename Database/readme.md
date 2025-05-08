# Database Directory

This directory contains SQL scripts for setting up and managing the databases required by the project.

## Requirements

- **MICROSOFT SQL SERVER 2022**

## Structure

- **linux/**
  - SQL scripts for Linux-based database servers.
- **windows/**
  - SQL scripts for Windows-based database servers.

Each subdirectory includes:

- `LosaAdmin.sql` – Schema and data for the admin database.
- `LosaGame.sql` – Schema and data for the main game database.
- `LosaGame_Log.sql` – Schema and data for game logging.
- `LosaLogData.sql` – Schema and data for additional log data.

## Usage

1. Select the appropriate folder (`windows` or `linux`) for your server environment.
2. Create new database user login lstggame and lstglog (restart SQL server after create)
3. Execute the SQL scripts in your database server in the following order:
   1. `LosaAdmin.sql`
   2. `LosaGame.sql`
   3. `LosaGame_Log.sql`
   4. `LosaLogData.sql`
4. Ensure your database user has privileges to create databases, tables, and insert data.

## Notes

- Scripts may contain platform-specific syntax or settings.
- Review and adjust scripts as needed for your environment or database version.

# Home Assistant Custom Add-on Repository: MariaDB Recorder Backend

This repository contains a production-ready Home Assistant custom add-on that helps you run Home Assistant Recorder on MariaDB instead of SQLite.

Repository URL to add in Home Assistant:

`https://github.com/chmajster/home-assistant-DataBase-Manage-automation`

## Included add-on

- **MariaDB Recorder Backend** (`mariadb_recorder`)
  - `internal_mariadb` mode: runs and maintains local MariaDB inside the add-on.
  - `external_mariadb` mode: validates and prepares connection details for your own external MariaDB.

## Add repository to Home Assistant

1. Open **Settings -> Add-ons -> Add-on Store**.
2. Click the three-dot menu (top-right) -> **Repositories**.
3. Add the repository URL.
4. Install **MariaDB Recorder Backend**.

## Documentation

- English add-on docs: [`mariadb_recorder/README.md`](mariadb_recorder/README.md)
- Polish docs: [`README.pl.md`](README.pl.md)

## Repository layout

- `repository.yaml` - Home Assistant add-on repository metadata
- `mariadb_recorder/` - add-on source code and documentation

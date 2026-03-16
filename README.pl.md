# Home Assistant Custom Add-on Repository: MariaDB Recorder Backend (PL)

To repozytorium zawiera gotowy custom add-on dla Home Assistanta, ktory pozwala uzywac MariaDB jako backendu `recorder` zamiast SQLite.

URL repozytorium do dodania w Home Assistant:

`https://github.com/chmajster/home-assistant-DataBase-Manage-automation`

## Co robi dodatek

Dodatek dziala w dwoch trybach:

1. **`internal_mariadb`**
   - uruchamia lokalna instancje MariaDB w kontenerze dodatku,
   - inicjalizuje trwaly katalog danych,
   - tworzy baze i uzytkownika dla Home Assistanta,
   - utrzymuje baze po restartach i aktualizacjach dodatku.

2. **`external_mariadb`**
   - uzywa podanych przez uzytkownika parametrow polaczenia,
   - sprawdza dostepnosc zewnetrznej bazy,
   - generuje gotowy `db_url` do sekcji `recorder`.

## Instalacja repozytorium i dodatku

1. W Home Assistant przejdz do **Ustawienia -> Dodatki -> Sklep dodatkow**.
2. Otworz menu (trzy kropki) -> **Repozytoria**.
3. Dodaj URL tego repozytorium.
4. Zainstaluj dodatek **MariaDB Recorder Backend**.

## Dokumentacja dodatku

Pelna dokumentacja konfiguracji dodatku:
- `mariadb_recorder/README.pl.md`
- `mariadb_recorder/README.md`

## Struktura repozytorium

- `repository.yaml` - metadane repozytorium add-onow
- `mariadb_recorder/` - kod dodatku, konfiguracja, skrypty i dokumentacja

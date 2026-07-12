# Mini-RIS - System Zarządzania Bazą Pacjentów i Badań
Program na wzór Radiologicznego Systemu Informatycznego, połączony z bazą danych PostgreSQL.

## Funkcje systemu
* Wprowadzanie nowych pacjentów, lekarzy, skierowań i badań do bazy
* Przechowywanie specjalnych własności badań, zależnych od rodzaju badania (np. dawka promieniowania, projekcja etc.)
* Zmiana istniejących danych w bazie
* Przeszukiwanie bazy
* Raport dzienny Zakładu

## Technologia
* **Język:** Python 3.x
* **Baza danych:** PostgreSQL
* **Biblioteki:** psycopg2, os, dotenv, datetime, matplotlib

## Uruchomienie i konfiguracja
1. Klonowanie repozytorium
Pobierz projekt na swój komputer za pomocą komendy:
``` bash
git clone https://github.com/Paulina-Slomczynska/Mini-RIS.git
cd Mini-RIS bash
``` 
2. Instalacja bibliotek
Zainstaluj wymagane biblioteki komendą:
``` bash
pip install -r requirements.txt
```
3. Przygotowanie bazy danych
* Otwórz DBeaver (oraz upewnij się, że serwer PostgreSQL działa) i stwórz nową, pustą bazę danych.
* Skopiuj i uruchom w niej zawartość pliku schema.sql, aby automatycznie stworzyć wszystkie potrzebne tabele i relacje.

4. Konfiguracja połączenia
* Stwórz plik .env w głównym folderze projektu (możesz skopiować wzór z pliku .env.example).
* Otwórz plik .env i wpisz swoje własne dane dostępowe do bazy danych:
```bash
DB_NAME=nazwa_twojej_bazy
DB_USER=twój_użytkownik
DB_PASSWORD=twoje_hasło
DB_HOST=localhost
DB_PORT=5432
```
5. Uruchomienie
Uruchom program komendą
``` bash
python mini_ris
```

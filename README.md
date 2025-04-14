# 🧸 ToysController – system zarządzania zabawkami

**ToysController** to aplikacja webowa dla rodziców, umożliwiająca:
- zarządzanie zabawkami dzieci,
- monitorowanie ich statusów,
- oznaczanie tagami,
- śledzenie terminów zwrotu (np. pożyczono),
- oraz przeglądanie danych przez REST API.

Projekt powstał z myślą o organizacji zabawek w rodzinie. Użytkownicy logują się przez Basic Auth i mają indywidualny limit przypisanych zabawek.

---

## 🚀 Funkcje

- 🔐 **Logowanie przez Basic Auth** (Spring Security)
- 👨‍👩‍👧 **Użytkownicy (rodzice)** z limitem zabawek
- 👶 **Dzieci** przypisane do rodziców
- 🧸 **Zabawki**:
  - przypisane do dziecka
  - statusy: `IN_USE`, `FOR_SALE`, `GIVEAWAY`, `BORROWED`
  - opcjonalnie: wypożyczenie, termin zwrotu
- 🏷️ **Tagowanie zabawek** – relacja wiele-do-wielu
- 📬 **Powiadomienia o zbliżającym się terminie zwrotu**
- 📚 **Swagger/OpenAPI** – pełna dokumentacja endpointów
- 🧪 **Plikami `.http`** ze środowiskami użytkowników

---

## ⚙️ Technologie

- Java 17
- Spring Boot
- Spring Security
- Spring Data JPA
- MySQL
- Lombok
- Swagger (OpenAPI 3)
- IntelliJ IDEA (wbudowany HTTP Client)

---

## 🔧 Uruchomienie

1. **Sklonuj repozytorium**

```bash
git clone https://github.com/twoj-login/ToysController.git
cd ToysController

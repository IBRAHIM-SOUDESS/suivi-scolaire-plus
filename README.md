# Suivi Scolaire Plus

> Web-based academic tracking platform connecting schools and parents with structured, real-time visibility into student performance.

**License:** [MIT](./LICENSE) · **Security Policy:** [SECURITY.md](./SECURITY.md)

---

## Overview

**Suivi Scolaire Plus** streamlines academic communication between school administrators and parents by centralizing student records, grade consultations, and institutional settings behind an authenticated web interface.

### Core Capabilities
- **Authentication & Access Guard** (`login.php`, `logout.php`, `auth_check.php`) — Session-protected administrative workspace.
- **Student Registry Management** (`ajout_eleve.php`, `liste_eleves.php`, `modifier_eleve.php`) — Full CRUD lifecycle for student profiles.
- **Academic Results Portal** (`resultat.php`) — Structured consultation of student grades and academic tracking.
- **School Configuration** (`parametres.php`) — Centralized institutional metadata and branding.

---

## Stack & Structure

- **Backend:** PHP 8 (`db.php`)
- **Database:** MySQL / MariaDB (`database.sql`)
- **Frontend:** Semantic HTML5, custom CSS (`style.css`)

```text
suivi-scolaire-plus/
├── auth_check.php       # Session authentication middleware
├── db.php               # Database connection layer
├── database.sql         # Relational schema definition
├── index.php            # Main dashboard entry point
├── ajout_eleve.php      # Student creation workflow
├── liste_eleves.php     # Student directory & overview
├── modifier_eleve.php   # Student record update workflow
├── resultat.php         # Academic results consultation
└── parametres.php       # Institutional settings
```

---

## Local Setup

1. Import `database.sql` into your local MySQL/MariaDB server.
2. Configure database credentials in `db.php`.
3. Serve the project with PHP's built-in server or Apache/Nginx:
   ```bash
   php -S localhost:8080
   ```

---

## Security & License

- Responsible vulnerability reporting: see [SECURITY.md](./SECURITY.md).
- Released under the [MIT License](./LICENSE).

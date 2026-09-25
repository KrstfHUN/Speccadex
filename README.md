# Speccadex

Speccadex egy PC-konfigurátor és közösségi platform, amely lehetővé teszi a felhasználók számára, hogy virtuálisan összeállítsák saját gépkonfigurációjukat egy adatbázisban tárolt alkatrészlistából, elmentsék ezeket későbbi felhasználásra, és megosszák a közösséggel egy beépített fórumon keresztül.

A rendszer valós (akár használt) árakkal dolgozik, hogy a felhasználók a saját budgetjükön belül tudjanak tervezni, és beépített bottleneck- és kompatibilitás-ellenőrzővel segíti, hogy csak életképes, kiegyensúlyozott konfigurációk szülessenek.

A platform három felületen érhető el — webes, asztali és mobil alkalmazásként —, közös adatbázisra épülve.

## Fő funkciók

-  Regisztráció / bejelentkezés, elmenthető konfigurációk
-  Alkatrész-adatbázis (új és használt árakkal)
-  Virtuális géptervezés / build-összeállítás
-  Bottleneck- és kompatibilitás-ellenőrző
-  Fórum: buildek megosztása, hozzászólás, mások buildjeinek elmentése
-  Admin panel: felhasználó-kezelés, alkatrész-feltöltés, fórum-moderáció

## Platformok

| Platform | Technológia |
|---|---|
| Web | React + Tailwind CSS (frontend), NestJS (backend) |
| Asztali alkalmazás | WPF |
| Mobil alkalmazás | Kotlin (Android) |

## Tech stack

**Web frontend**
- React
- Tailwind CSS

**Web backend**
- NestJS (Node.js / TypeScript)
- Drizzle ORM
- Swagger / OpenAPI dokumentáció
- JWT + Passport.js autentikáció

**Adatbázis**
- PostgreSQL

**Asztali alkalmazás**
- WPF (.NET / C#)

**Mobil alkalmazás**
- Kotlin (Android)

## Csapat

| Név | Felelősségi kör | Tudás |
|---|---|---|
| Tóth Kristóf Antal | Web alkalmazás (React/Tailwind + NestJS) | React, NestJS, Tailwind CSS, PostgreSQL |
| Vincze Dominik | Asztali alkalmazás (WPF) | WPF, C#/.NET |
| Papp-hegyi Ákos | Mobil alkalmazás (Kotlin) | Kotlin, Android fejlesztés |

Az adatbázis tervezése és fejlesztése közös munkával történik.

## Projekt struktúra

```
speccadex/
├── web/            # React + Tailwind frontend
├── api/            # NestJS backend
├── desktop/        # WPF asztali alkalmazás
├── mobile/         # Kotlin (Android) alkalmazás
└── database/       # Közös adatbázis-séma / migrációk
```

## Fejlesztői környezet beállítása

> A pontos lépések a fejlesztés előrehaladtával frissülnek.

### Előfeltételek
- Node.js (LTS)
- PostgreSQL
- .NET SDK (asztali alkalmazáshoz)
- Android Studio / Kotlin toolchain (mobil alkalmazáshoz)

### Web backend indítása
```bash
cd api
npm install
npm run start:dev
```

### Web frontend indítása
```bash
cd web
npm install
npm run dev
```

## Licenc

Ez a projekt oktatási célból készül.

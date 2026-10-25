# Employee CRUD – Front End (MyEmployeeCrud)

Angular single-page application that lists, creates, updates and deletes employees (name, mobile number, e-mail) by calling a REST API.

## Tech stack

- Angular 14 (Angular CLI 14.2), TypeScript
- Bootstrap 5

## Folder structure

```text
Employee-Crud-FrontEnd/
├── .vscode/
├── src/
│   ├── app/
│   │   ├── models/
│   │   └── service/
│   ├── assets/
│   ├── environments/
│   ├── index.html
│   └── main.ts
├── .browserslistrc
├── .editorconfig
├── .gitignore
├── angular.json
├── karma.conf.js
├── package-lock.json
├── package.json
├── README.md
├── tsconfig.app.json
├── tsconfig.json
└── tsconfig.spec.json
```

| Path | Purpose |
| --- | --- |
| `src/app/app.component.*` | Employee list and form |
| `src/app/service/employee.service.ts` | HTTP calls (GET, POST, PUT, DELETE) |
| `src/app/models/employee.ts` | `Employee` model |

## Prerequisites

- Node.js 14.20+, 16.13+ or 18.10+ (supported by Angular 14) and npm
- An Employee REST API (not part of this repository) exposing `GET/POST/PUT/DELETE` on `https://localhost:7223/api/Employee`

## Configuration

The API URL is set in `src/app/service/employee.service.ts` (`baseurl`). Change it there if your API runs on a different address.

## Running locally

```bash
npm install
npm start          # ng serve → http://localhost:4200
```

## Build and test

```bash
npm run build      # output in dist/
npm test           # Karma + Jasmine
```

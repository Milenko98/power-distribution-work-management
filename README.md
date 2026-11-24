# Power Distribution Work Management – university team project

Web application for managing field work in a power distribution network: work requests, work plans, safety documents, field teams and a network map.
Built in 2021 as a team project (3 students) for the *PUSGS* course at the **Faculty of Technical Sciences, Novi Sad**.

## Features

- **Registration and login** – JWT authentication and **Google sign-in**, account verification and route guards.
- **Work requests** – basic information, equipment, multimedia attachments and full history of changes.
- **Documents** – work plans and safety documents.
- **Teams** – create field teams and assign members.
- **Map** – network elements displayed on an interactive OpenLayers map (GeoJSON).
- **Dashboard and notifications** – overview charts and toast notifications.

## My contribution

- Project setup and application core (Angular structure, layout, routing)
- Registration and login, including JWT and Google sign-in on the backend
- Backend foundation (ASP.NET Core Web API, Entity Framework Core, data model)
- Work requests – frontend and backend
- Teams and route guards
- Interactive map and assigning teams

## Tech stack

| Layer    | Technologies |
|----------|--------------|
| Frontend | Angular 11, TypeScript, Angular Material, Bootstrap, OpenLayers, Chart.js, ngx-toastr |
| Backend  | C#, ASP.NET Core 2.1 Web API, Entity Framework Core, SQL Server, JWT, Google OAuth |

## Project structure

```
PUSGS/        # Angular frontend – components, services, entities, guards
PUSGSVeb2/    # ASP.NET Core Web API – controllers (User, Team, WorkRequest, UploadFiles), EF models
PUSGSVS/      # initial backend prototype
```

## Running locally

**Backend** – open `PUSGSVeb2/PUSGSVeb2.sln`, set the connection string and `JWT_Secret` in `appsettings.json`, apply EF migrations and run.

**Frontend**

```bash
cd PUSGS
npm install
npx ng serve      # http://localhost:4200
```

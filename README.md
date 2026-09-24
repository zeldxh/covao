# covao

School cafeteria management system built for COVAO's cafeteria. A PHP web application for managing student cafeteria services, meals, billing, and attendance tracking.

## Features

- Role-based access: administrator, billing staff, and client (student/teacher)
- Student and teacher management with Excel bulk import
- Meal attendance tracking and billing
- Non-school day calendar management
- Statistics dashboard
- Profile photo uploads
- Automated password generation and email notifications

## Setup

There are three ways to run this project. Pick whichever fits your environment:

| Option | What you install locally | Guide |
|--------|------------------------|-------|
| Pure PHP + MySQL | PHP, MySQL | [Getting started, option A](docs/getting-started.md#option-a-pure-php--mysql) |
| DB only in Docker | PHP, Docker | [Getting started, option B](docs/getting-started.md#option-b-php-local--mysql-in-docker) |
| Full Docker | Docker | [Docker guide](docs/docker-guide.md) |

## Tech Stack

- PHP 8.x (no frameworks, no Composer dependencies)
- MySQL 8.0
- Bootstrap 5.1.3, Font Awesome, AlertifyJS
- Vanilla JavaScript

## Project Structure

```
index.php           entry point
Core/               router, constants, config
Controller/         mvc controllers
  admin/            admin crud controllers
  billing/          billing controllers
  client/           client-facing controllers
  helpers/          utility controllers
Model/              mvc models
  Connection.php    database connection
  Entities/         entity classes
  Methods/          data access classes
View/               mvc views
  views/            php templates
  css/              stylesheets
  js/               javascript
  assets/           images, audio, favicons
docs/               documentation
```

## License

MIT License, see [LICENSE](LICENSE).

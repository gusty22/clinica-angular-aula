# App

This project was generated using [Angular CLI](https://github.com/angular/angular-cli) version 20.3.9.

## Development server

To start a local development server, run:

```bash
ng serve
```

Once the server is running, open your browser and navigate to `http://localhost:4200/`. The application will automatically reload whenever you modify any of the source files.

## Code scaffolding

Angular CLI includes powerful code scaffolding tools. To generate a new component, run:

```bash
ng generate component component-name
```

For a complete list of available schematics (such as `components`, `directives`, or `pipes`), run:

```bash
ng generate --help
```

## Building

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.



-- criar o diretório

mkdir meu-app-angular

-- entrar no diretório

cd meu-app-angular

-- criar o contâiner
Linux: docker run -it --rm -v "${PWD}:/app" -w /app node:20-alpine sh
  windows: docker run -it --rm -v "%cd%:/app" -w /app node:20-alpine sh

-- instalar o angular e criando uma aplicação

  npx @angular/cli new clinica --directory . --skip-git

-- mostrar as pastas dentro do container

rm -rf *

-- sair depois da execução

exit

-- rodar aplicação
linux: docker run -it --rm -v "${PWD}:/app" -w /app -p 4200:4200 node:20-alpine npx ng serve --host 0.0.0.0 --poll=2000 
windows:docker run -it --rm -v "%cd%:/app" -w /app -p 4200:4200 node:20-alpine npx ng serve --host 0.0.0.0 --poll=2000

docker run -it --rm -v "%CD%":/app -w /app node:20-alpine sh

ng generate module administrativo
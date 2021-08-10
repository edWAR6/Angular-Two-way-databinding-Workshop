# Taller de Angular

![Resultado](/images/result.png)

Autor: Eduardo Oviedo Blanco

Para usar este taller efectivamente, clone el código en su ambiente local.
```
git clone https://github.com/edWAR6/Angular-Two-way-databinding-Workshop.git
```
Si desea subir el taller en su repositorio personal.
Cree un repositorio en su perfil, luego:
```
git remote set-url origin https://github.com/<su usuario>/angular-two-way-databinding-workshop.git
```

> El nombre del repositorio puede cambiar. Siga las instrucciones y guarde sus cambios.

## Propósito

Este taller demuestra el uso de Angular two-way databinding.

## Instrucciones

1. Ejecute el proyecto desde el inicio para que vea los cambios según avanza.

```bash
ng serve
```

2. Agregue (en la línea 11) la propiedad ngModel.
```html
<input class="form-control mt-2" type="text"
    [(ngModel)]="query">
```

3. Note que hay un error y para solucionarlo incluya el módulo correspondiente en `app.module.ts`.

```typescript
import { FormsModule } from '@angular/forms';
```

4. También agréguelos a la lista de imports.
```typescript
  imports: [
    BrowserModule,
    AppRoutingModule,
    FormsModule
  ],
```

> Note como ahora el query tiene un Two-way Databinding.

# angularTwoWayDatabinding

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.

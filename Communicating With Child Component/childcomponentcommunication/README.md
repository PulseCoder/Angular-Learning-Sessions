# Childcomponentcommunication

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.2.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

=======================================================================================================================================================================================

Communicating with the child component.

Step 1: Declare the child component selector in the parent component html.
Step 2: Now in order to access the parent component data that is available in the parent component ts file has to used in the child component selector like below explained.
            <app-child [childData]="child"></app-child>
            Here child refers to the variable in the parent component ts file.
            Here childData refers to the variable in the child component ts file which will accept data from the parent component.
Step 3: Now in the child component ts file 
            @Input() childData; 
            This @Input() which is available in @angular/core field available in the child component will accept data.
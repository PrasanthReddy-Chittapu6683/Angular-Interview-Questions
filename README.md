# Angular Interview Questions

## 1.  What is Angular Framework?
   * Angular is a TypeScript-based open-source front-end platform that makes it easy to build applications with in web/mobile/desktop. The major features of this framework such as  declarative templates, dependency injection, end to end tooling, and many more other features are used to ease the development.

## 2. What is the difference between AngularJS and Angular?
   * Angular is a completely revived component-based framework in which an application is a tree of individual components.
   * Some of the major difference in tabular form
    ![](./images/Q2.PNG)

## 3. What is TypeScript?
   *   TypeScript is a typed superset of JavaScript created by Microsoft that adds optional types, classes, async/await, and   many other features, and compiles to plain JavaScript. Angular built entirely in TypeScript and used as a primary language. You can install it globally as
   ``` javascript
       npm install -g typescript
   ```
   * Let's see a simple example of TypeScript usage:

    ``` javascript
      function greeter(person: string) {
          return "Hello, " + person;
      }
      let user = "Sudheer";
      document.body.innerHTML = greeter(user);
    ```
## 4. Write a pictorial diagram of Angular architecture?
   *  ![](./images/Q4.PNG)

## 5. What are the key components of Angular?
   * Angular has the below key components,
        i.	Component: These are the basic building blocks of angular application to control HTML views.
        ii.	Modules: An angular module is set of angular basic building blocks like component, directives, services etc. An   application is divided into logical pieces and each piece of code is called as "module" which perform a single task.
        iii.	Templates: This represent the views of an Angular application.
        iv.	Services: It is used to create components which can be shared across the entire application.
        v.	Metadata: This can be used to add more data to an Angular class.
## 6. What are directives?
   * Directives add behavior to an existing DOM element or an existing component instance.
        ``` javascript
         import { Directive, ElementRef, Input } from '@angular/core';

           @Directive({ selector: '[myHighlight]' })
           export class HighlightDirective {
               constructor(el: ElementRef) {
                 el.nativeElement.style.backgroundColor = 'yellow';
               }
           }
       ```
   * Now this directive extends HTML element behavior with a yellow background as below
         ``` javascript
           <p myHighlight>Highlight me!</p>
         ```

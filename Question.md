#Angular Interview Question
### What is Angular ?
Angular is a TypeScript-based, free and open-source single-page web application framework led by the Angular Team at Google and by a community of individuals and corporations
Angular includes:

A component-based framework for building scalable web applications
A collection of well-integrated libraries that cover a wide variety of features, including routing, forms management, client-server communication, and more
A suite of developer tools to help you develop, build, test, and update your code

### What is Component ?
Components are the fundamental building block for creating applications in Angular. By leveraging component architecture, Angular aims to provide structure for organizing your project into manageable, well organized parts with clear responsibilities so that your code is maintainable and scalable.

An Angular component can be identified by the component suffix (e.g., my-custom-name.component.ts and has the following:

A decorator to define configuration options for things like:
A selector that defines what the tag name is when referring a component in a template
An HTML template that controls what is rendered to the browser
A TypeScript class that defines the behavior of the component. Examples include handling user input, managing state, defining methods, etc.

##Example of component 
```
// 📄 todo-list-item.component.ts
@Component({
  standalone: true,
  selector: 'todo-list-item',
  template: ` <li>(TODO) Read cup of coffee introduction</li> `,
  styles: ['li { color: papayawhip; }'],
})
export class TodoListItem {
  /* Component behavior is defined in here */
}
```
## Angular cli Commands 
```
ng serve -o //to run the project in localhost

```
What are the key components of Angular?
Angular has the key components below,
Component: These are the basic building blocks of an Angular application to control HTML views.
Modules: An Angular module is a set of angular basic building blocks like components, directives, services etc. An application is divided into logical pieces and each piece of code is called as "module" which perform a single task.
Templates: These represent the views of an Angular application.
Services: Are used to create components which can be shared across the entire application.
Metadata: This can be used to add more data to an Angular class.

What is a module?
Modules are logical boundaries in your application and the application is divided into separate modules to separate the functionality of your application. Lets take an example of app.module.ts root module declared with @NgModule decorator as below,
```
import { NgModule }      from '@angular/core';
import { BrowserModule } from '@angular/platform-browser';
import { AppComponent }  from './app.component';

@NgModule ({
   imports:      [ BrowserModule ],
   declarations: [ AppComponent ],
   bootstrap:    [ AppComponent ],
   providers: []
})
export class AppModule { }
```

The NgModule decorator has five important (among all) options:

The imports option is used to import other dependent modules. The BrowserModule is required by default for any web based angular application.
The declarations option is used to define components in the respective module.
The bootstrap option tells Angular which Component to bootstrap in the application.
The providers option is used to configure a set of injectable objects that are available in the injector of this module.
The entryComponents option is a set of components dynamically loaded into the view.


What are lifecycle hooks available?
Angular application goes through an entire set of processes or has a lifecycle right from its initiation to the end of the application. 



The description of each lifecycle method is as below,

ngOnChanges: When the value of a data bound property changes, then this method is called.
ngOnInit: This is called whenever the initialization of the directive/component after Angular first displays the data-bound properties happens.
ngDoCheck: This is for the detection and to act on changes that Angular can't or won't detect on its own.
ngAfterContentInit: This is called in response after Angular projects external content into the component's view.
ngAfterContentChecked: This is called in response after Angular checks the content projected into the component.
ngAfterViewInit: This is called in response after Angular initializes the component's views and child views.
ngAfterViewChecked: This is called in response after Angular checks the component's views and child views.
ngOnDestroy: This is the cleanup phase just before Angular destroys the directive/component.

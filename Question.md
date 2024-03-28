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

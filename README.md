# Angular Non-Standalone Learning Roadmap

## Prerequisites
- **HTML/CSS**: Strong understanding of web fundamentals
- **JavaScript ES6+**: Arrow functions, classes, modules, async/await, destructuring
- **TypeScript**: Basic understanding of types, interfaces, classes
- **Node.js & npm**: Package management and basic CLI usage

## Phase 1: Foundation (Week 1-2)

### 1. Angular Architecture & Setup
- **Angular CLI**: Installation and project creation
- **Project Structure**: Understanding folders and files
- **Angular Modules**: NgModule decorator and module organization
- **Components**: Component lifecycle and basic structure
- **Templates**: HTML templates and basic data binding

### Key Concepts to Master:
```typescript
// App Module Structure
@NgModule({
  declarations: [AppComponent],
  imports: [BrowserModule],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }

// Component Structure
@Component({
  selector: 'app-example',
  templateUrl: './example.component.html',
  styleUrls: ['./example.component.css']
})
export class ExampleComponent { }
```

### 2. Data Binding & Interpolation
- **String Interpolation**: `{{ }}`
- **Property Binding**: `[property]`
- **Event Binding**: `(event)`
- **Two-way Binding**: `[(ngModel)]`

## Phase 2: Core Concepts (Week 3-4)

### 3. Directives
- **Structural Directives**: `*ngIf`, `*ngFor`, `*ngSwitch`
- **Attribute Directives**: `ngClass`, `ngStyle`
- **Custom Directives**: Creating your own directives

### 4. Component Communication
- **@Input()**: Parent to child communication
- **@Output()**: Child to parent communication with EventEmitter
- **ViewChild & ViewChildren**: Accessing child components
- **Template Reference Variables**: `#variableName`

### 5. Services & Dependency Injection
- **Creating Services**: `@Injectable()` decorator
- **Dependency Injection**: Constructor injection
- **Service Hierarchy**: Root, module, and component level
- **Singleton Services**: Understanding service instances

## Phase 3: Advanced Features (Week 5-6)

### 6. Routing & Navigation
- **Router Module**: Setting up routing
- **Route Configuration**: Path, component, redirects
- **Router Outlet**: `<router-outlet>`
- **Navigation**: `routerLink`, Router service
- **Route Parameters**: `ActivatedRoute`
- **Route Guards**: CanActivate, CanDeactivate

### 7. Forms
- **Template-driven Forms**: NgModel, form validation
- **Reactive Forms**: FormBuilder, FormGroup, FormControl
- **Form Validation**: Built-in and custom validators
- **Dynamic Forms**: Creating forms programmatically

### 8. HTTP Client
- **HttpClientModule**: Setup and configuration
- **HTTP Methods**: GET, POST, PUT, DELETE
- **Observables**: Understanding RxJS basics
- **Error Handling**: Catching and handling HTTP errors
- **Interceptors**: Request/response manipulation

## Phase 4: Advanced Topics (Week 7-8)

### 9. RxJS & Observables
- **Observable Patterns**: Subscribe, unsubscribe
- **Operators**: map, filter, switchMap, mergeMap
- **Subjects**: BehaviorSubject, ReplaySubject
- **Async Pipe**: Template subscription handling

### 10. Pipes
- **Built-in Pipes**: date, currency, json, async
- **Custom Pipes**: Creating transformation pipes
- **Pure vs Impure Pipes**: Performance considerations

### 11. Lifecycle Hooks
- **ngOnInit**: Component initialization
- **ngOnDestroy**: Cleanup and unsubscription
- **ngOnChanges**: Input property changes
- **ngAfterViewInit**: View initialization
- **Complete Lifecycle**: Understanding all hooks

## Phase 5: Architecture & Best Practices (Week 9-10)

### 12. Module Organization
- **Feature Modules**: Organizing by functionality
- **Core Module**: Singleton services
- **Shared Module**: Common components and pipes
- **Lazy Loading**: Route-based module loading

### 13. State Management
- **Component State**: Local state management
- **Service State**: Shared state through services
- **NgRx** (Optional): Redux pattern for complex apps

### 14. Testing
- **Unit Testing**: Jasmine and Karma setup
- **Component Testing**: TestBed configuration
- **Service Testing**: Dependency injection in tests
- **E2E Testing**: Protractor or Cypress basics

## Phase 6: Production & Optimization (Week 11-12)

### 15. Performance Optimization
- **Change Detection**: OnPush strategy
- **TrackBy Functions**: Optimizing *ngFor
- **Lazy Loading**: Module and image lazy loading
- **Bundle Analysis**: Understanding build output

### 16. Build & Deployment
- **Production Builds**: `ng build --prod`
- **Environment Configuration**: Development vs production
- **Deployment Strategies**: Static hosting, server deployment

## Hands-on Projects

### Project 1: Todo Application (Week 3-4)
- Components, services, local storage
- CRUD operations, form handling

### Project 2: Blog Application (Week 6-7)
- Routing, HTTP client, authentication
- Multiple modules, guards

### Project 3: E-commerce Dashboard (Week 9-10)
- Complex forms, data visualization
- State management, testing

## Learning Resources

### Official Documentation
- [Angular.io](https://angular.io) - Official documentation
- [Angular CLI](https://cli.angular.io) - Command line interface docs

### Practice Platforms
- **StackBlitz**: Online Angular development
- **CodeSandbox**: Quick prototyping
- **GitHub**: Version control and portfolio

### Additional Learning
- **Angular University**: Advanced courses
- **Pluralsight/Udemy**: Structured video courses
- **Angular Blog**: Official updates and best practices

## Daily Learning Schedule

### Week Structure (2-3 hours/day)
- **Monday-Wednesday**: New concepts and theory
- **Thursday-Friday**: Hands-on coding practice
- **Weekend**: Project work and review

### Study Tips
1. **Code Along**: Always practice while learning
2. **Build Projects**: Apply concepts immediately
3. **Read Documentation**: Official docs are comprehensive
4. **Join Community**: Angular Discord, Reddit, Stack Overflow
5. **Version Control**: Use Git from day one

## Common Pitfalls to Avoid

1. **Memory Leaks**: Always unsubscribe from Observables
2. **Module Imports**: Don't import modules multiple times
3. **Change Detection**: Understand when Angular updates views
4. **Async Operations**: Handle loading states and errors
5. **Type Safety**: Leverage TypeScript's type system

## Assessment Checkpoints

### Week 4: Basic Competency
- Create components and modules
- Implement data binding and directives
- Build simple forms

### Week 8: Intermediate Level
- Implement routing and navigation
- Work with HTTP services
- Create reactive forms

### Week 12: Advanced Understanding
- Optimize application performance
- Implement testing strategies
- Deploy production applications

## Next Steps After Completion

- **Advanced Angular**: Animations, CDK, Material
- **Backend Integration**: Node.js, .NET, Java APIs
- **Mobile Development**: Ionic framework
- **Desktop Development**: Electron integration
- **Micro-frontends**: Advanced architecture patterns

Remember: Angular has a steep learning curve, but the module-based architecture provides a solid foundation for large-scale applications. Focus on understanding the fundamentals before moving to advanced topics.

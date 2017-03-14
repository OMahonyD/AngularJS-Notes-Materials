# High-Level Overview - Angular Process
* AngularJS is included and executed.
* Angular module gets created (if added)
* Finds 'templates':
  * Template: HTML with some angular markup
    * 'ng-*' attributes (directives)
    * Evaluating expressions
    * data-binding markup etc.
* Processes template:
  * Compiles template (for errors)
  * Loads template (instance) in memory
  * Transforms template with data
    * data binding
    * Evaluation of expressions
* Renders to DOM tree (View)

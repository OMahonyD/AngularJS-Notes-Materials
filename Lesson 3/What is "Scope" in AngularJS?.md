# What is "Scope" in AngularJS?

### A Mediator

* Scope is made available directly as part of the controller.
* Whenever the controller needs to send info to the view, it does so through the scope.
* Simlarly if the view needs to send info back to the controller it goes through the scope.
* Scope is the mediator between the controller and the view.
  * Controller sends the information to the scope, scope sends it to the view and vice versa

* If a property is provided within {{}} that is not available within the scope (ie. hasn't been defined within the controller), there may not be any error message

### Using Angular "scope" within the controller

* $scope referenced as a parameter within the controller function
* $scope.Name  = "Jag" >> used as {{Name}} within view.

### Dev Tools

* AngularJS adds ng-scope and ng-binding
* Debugging in console - angular.element($0).scope()
* Modifying from the console:
  * angular.element($0).scope().name
    * changes the element value in the console but not in the actual view
  * In order to propagate the entire scope object back to the View you need to call:
    * angular.element($0).scope().$digest()

## Using Angular 'scope' - different syntaxes

* Different approaches - refer to video for examples. At the moment, use $scope

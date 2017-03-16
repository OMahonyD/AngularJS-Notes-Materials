# $rootScope and Scope Inheritance
  * Root Scope associated to module (ng-app)
  * Whether you define it or not, the rootScope is created once ng-app is created.
  * emp Scope nested within the ng-app (the rootScope)
  * empDetails scope nested within emp scope

## Using Root Scope as part of the Application?
  * Using .run() method concat after module declaration 
  * $rootScope.TaxPercent = 30;
  * This method made available to emp scope
  * empDetails also has TaxPercent available to it

## Modifying Root Scope
  * Imagine three scope adjacent to each other (e.g. at the same level as emp but not related)
  * Siblings of emp
  * Direct descendants of rootScope
  * TaxPercent will be made available to all of the children.

## If rootScope member modifies the TaxPercent, which it inherited from the rootScope:
  * That modification will be applicable everywhere.
  * Makes sense as we are referring to the same value everywhere

N.B. If values need to be shared, shy away from using rootScope value - BAD PRACTICE, only available as part of convenience.

## Accessing Root Scope in Controller

  * Consider the tax percent in the controller from the previous lesson.
  * $rootScope declared as part of the controller

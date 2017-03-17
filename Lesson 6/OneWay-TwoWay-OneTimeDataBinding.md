# Data Binding

## One-Way Data Binding
* Data flows from "Scope" to "View"
* Scope Data
  * Gets propagated to View
  * Data Modifications: propagated immediately and reflected in View
* View Data
  * No propagation happens (back to scope) for any data change
* Usually performed through "ng-bind" or evaluating expressions {{}}

## Two-Way Data Binding
* Data flows from "Scope" to "View" and vice versa
* Scope Data
  * Gets propagated to View
  * Data modifications: propagated immediately and reflected in View
* View Data
  * Gets propagated to Scope
  * Data modifications: propagated immediately and reflected in Scope
* Usually performed through "ng-model"

## One-Time Data Binding
* Data flows from "Scope" to "View"
* Scope Data
  * Gets propagated to View (only once for the first time)
  * Data modifications: No propagation.
* View Data:
  * No propagation happens (back to scope) for any data change.
  * Usually performed through "::" as part of evaluating expressions.

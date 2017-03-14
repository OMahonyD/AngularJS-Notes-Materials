# AngularJS Controllers

* Controllers are JavaScript objects which contain application logic:
  * Usually defined as part of angular module
  * Controllers attached to the module by directly referring to the module instance
    * Give controller name as first argument.
    * Second argument is a function which contains the definition of the controller
* Controllers allow for data to be sent/received between DOM (the "Views") and the application logic.
* Controller is usually attached to a DOM element using 'ng-controller' attribute (directive)
  * Gets instantiated
* In other words, the controller exposes data (Model) to be consumed by Views (one-way data-binding)
  * Also sends/takes data from Views (two-way data-binding) - cover later.

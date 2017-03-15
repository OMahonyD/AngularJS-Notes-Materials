# Scope Inheritance

* Scopes nested - emp and empDetails
  * {{Name}} attribute in emp
  * empDetails controller nested within emp
  * {{Name}} is made available to the inner scope through inheritance
  * NB: Attributes defined within empDetails not available to the higher level scope
  * If, for example, there are two definitions of {{Name}}, one within outer scope (emp) and another within inner scope (empDetails):
    * Binding within the <div> for which empDetails controller will use the inner scope {{Name}}
    * If {{Name}} not defined within the inner scope - <div> for which empDetails is responsible will look outside to emp and use that
 
* Check Example 4 and use console to understand better. techCBT is a great teacher!




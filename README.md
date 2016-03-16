Angular Hide Header Extended
============================

Angular directive for hiding a header when scrolling down and showing it when scrolling up.

##### This is an extended version of Mario Flores's directive: https://github.com/pokaxperia/angular-hide-header

Demo
-------
Check out [the live demo](http://run.plnkr.co/plunks/ePnxK2).

Installation
-------

#### via bower:

```
$ bower install angular-hide-header-extended --save
```

Usage
---

1. Include **angularHideHeaderExtended** as a dependency for your app

  ```
  angular.module('myApp', ['angularHideHeaderExtended'])
  ```
  
2. Easy, add the directive to header element you want to hide or show.

    ```
    <header hide-header hide-header-on="true">
    </header>
    ```
     This is the most basic example.
  
Configuration
--- 
*  Add **hide-offset** to specify from which pixels from the top header will hide. Default value is 60.

    hide-offset="80"  
     
     ```
      <header hide-header hide-offset="80">
      </header>
      ```

*  Add **hide-header-on** to bind to a scope variable that controls if the header is to be hidden or not.

    hide-header-on="true" // default behaviour
    hide-header-on="hideHeader" // default behaviour   
    
    ```
  <header hide-header hide-header-on="hideHeader">
  ```
  ```
  Hide Header? <input type="checkbox" ng-model="hideHeader" />
  ```
  ```
  </header>
  ```

---------

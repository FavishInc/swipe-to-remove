angularApApp
============

to run demo install dependencies
```
cd demo
npm install
bower install
```
run the server
```
grunt server


Usage
in HTML
```
<div item-swipe on-remove="removeThing(thing)" ng-repeat="thing in things">{{thing.name}}</div>

in controller
```
$scope.removeThing = function(thing){
  $scope.things.splice($scope.things.indexOf(thing), 1);
};
```
# Angular.js Snippets for Sublime Text 2

This snippet library provides completions for Angular.js’s stable and unstable branch.
Sublime Text uses fuzzy searching for snippets in JavaScript therefore you don’t have to write the complete trigger.

## Installation

- Package Control: install the package "AngularJS Snippets" (not yet available)
- Manual: copy files to the Sublime packages folder

## IMPORTANT

Completions won’t show in HTML unless you have added this line to your User.sublime-preferences:

	"auto_complete_triggers": [ {"selector": "text.html", "characters": "<"}, {"selector": "source.js", "characters": "$." }, {"selector": "text.html meta.tag", "characters": " " } ]

This line also ensures to show completions whenever you have entered $ oder . in a JavaScript file.

__Snippet Categories:__
- [Directives](#directives)
- [Globals](#globals)
- [Services](#services)
- [Variables](#variables)

## Directives

Note: triggers are chosen by Sublime Text’s __fuzzy searching__ so you don’t have to type them completely.

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>ng-animate</th><td>ng-animate="{enter: '{example}-enter', leave: '{example}-leave'}"</td></tr>
	<tr><th>ng-animates</th><td>ng-animate="'{class-prefix}'"</td></tr>
	<tr><th>ng-app</th><td>ng-app="|"</td></tr>
	<tr><th>ng-bind</th><td>ng-bind="|"</td></tr>
	<tr><th>ng-bind-html-unsafe</th><td>ng-bind-html-unsafe="|"</td></tr>
	<tr><th>ng-bind-template</th><td>ng-bind-template="|"</td></tr>
	<tr><th>ng-change</th><td>ng-change="|"</td></tr>
	<tr><th>ng-checked<span style="color: green">a</span></th><td>ng-checked="|"</td></tr>
	<tr><th>ng-class<span style="color: green">a</span></th><td>ng-class="|"</td></tr>
	<tr><th>ng-class-even</th><td>ng-class-even="|"</td></tr>
	<tr><th>ng-class-odd</th><td>ng-class-odd="|"</td></tr>
	<tr><th>ng-click</th><td>ng-click="|"</td></tr>
	<tr><th>ng-cloak</th><td>ng-cloak</td></tr>
	<tr><th>ng-controller</th><td>ng-controller="{Name}Ctrl"</td></tr>
	<tr><th>ng-dblclick</th><td>ng-dblclick="|"</td></tr>
	<tr><th>ng-disabled<span style="color: green">a</span></th><td>ng-disabled="|"</td></tr>
	<tr><th>ng-form<span style="color: green">a</span></th><td>ng-form="|"</td></tr>
	<tr><th>ng-hide</th><td>ng-hide="|"</td></tr>
	<tr><th>ng-href<span style="color: green">a</span></th><td>ng-href="|"</td></tr>
	<tr><th>ng-if</th><td>ng-if="|"</td></tr>
	<tr><th>ng-include</th><td>ng-include="{template}" {onload="|" autoscroll="|"}</td></tr>
	<tr><th>ng-init</th><td>ng-init="|"</td></tr>
	<tr><th>ng-keydown</th><td>ng-keydown="|"</td></tr>
	<tr><th>ng-keypress</th><td>ng-keypress="|"</td></tr>
	<tr><th>ng-keyup</th><td>ng-keyup="|"</td></tr>
	<tr><th>ng-list</th><td>ng-list="|"</td></tr>
	<tr><th>ng-model</th><td>ng-model="|"</td></tr>
	<tr><th>ng-mousedown</th><td>ng-mousedown="|"</td></tr>
	<tr><th>ng-mouseenter</th><td>ng-mouseenter="|"</td></tr>
	<tr><th>ng-mouseleave</th><td>ng-mouseleave="|"</td></tr>
	<tr><th>ng-mousemove</th><td>ng-mousemove="|"</td></tr>
	<tr><th>ng-mouseover</th><td>ng-mouseover="|"</td></tr>
	<tr><th>ng-mouseup</th><td>ng-mouseup="|"</td></tr>
	<tr><th>ng-multiple</th><td>ng-multiple="|"</td></tr>
	<tr><th>ng-nbind</th><td>ng-non-bindable="|"</td></tr>
	<tr><th>ng-open</th><td>ng-open="|"</td></tr>
	<tr><th>ng-pluralize</th><td>ng-pluralize count="|" when="'|': '{}'"</td></tr>
	<tr><th>ng-readonly<span style="color: green">a</span></th><td>ng-readonly="|"</td></tr>
	<tr><th>ng-repeat</th><td>ng-repeat="{item} in {array}"</td></tr>
	<tr><th>ng-selected<span style="color: green">a</span></th><td>ng-selected="|"</td></tr>
	<tr><th>ng-show</th><td>ng-show="|"</td></tr>
	<tr><th>ng-src<span style="color: green">a</span></th><td>ng-src="|"</td></tr>
	<tr><th>ng-style<span style="color: green">a</span></th><td>ng-style="|"</td></tr>
	<tr><th>ng-submit</th><td>ng-submit="|"</td></tr>
	<tr><th>ng-swipeleft</th><td>ng-swipe-left="|"</td></tr>
	<tr><th>ng-swiperight</th><td>ng-swipe-right="|"</td></tr>
	<tr><th>ng-switch</th><td>ng-switch on="|"</td></tr>
	<tr><th>ng-switchd</th><td>ng-switch-default="|"</td></tr>
	<tr><th>ng-switchw</th><td>ng-switch-when="|"</td></tr>
	<tr><th>ng-transclude</th><td>ng-transclude</td></tr>
	<tr><th>ng-view</th><td>ng-view</td></tr>
</table>

## Globals

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular.bind</th><td><pre>angular.bind({self}, {function}|)</pre></td></tr>
	<tr><th>angular.bootstrap</th><td><pre>angular.bootstrap({element}{, [{modules}]})</pre></td></tr>
	<tr><th>angular.copy</th><td><pre>angular.copy({source}{, {destination}})</pre></td></tr>
	<tr><th>angular.element</th><td><pre>angular.element({element})</pre></td></tr>
	<tr><th>angular.equals</th><td><pre>angular.equals({obj1}, {obj2})</pre></td></tr>
	<tr><th>angular.extend</th><td><pre>angular.extend({destination}, {source})</pre></td></tr>
	<tr><th>angular.forEach</th><td><pre>angular.forEach({obj}, {iterator}|)</pre></td></tr>
	<tr><th>angular.fromJson</th><td><pre>angular.fromJson({jsonString})</pre></td></tr>
	<tr><th>angular.identity</th><td><pre>angular.identity()</pre></td></tr>
	<tr><th>angular.injector</th><td><pre>angular.injector([{modules}])</pre></td></tr>
	<tr><th>angular.isArray</th><td><pre>angular.isArray({value})</pre></td></tr>
	<tr><th>angular.isDate</th><td><pre>angular.isDate({value})</pre></td></tr>
	<tr><th>angular.isDefined</th><td><pre>angular.isDefined({value})</pre></td></tr>
	<tr><th>angular.isElement</th><td><pre>angular.isElement({value})</pre></td></tr>
	<tr><th>angular.isFunction</th><td><pre>angular.isFunction({value})</pre></td></tr>
	<tr><th>angular.isNumber</th><td><pre>angular.isNumber({value})</pre></td></tr>
	<tr><th>angular.isObject</th><td><pre>angular.isObject({value})</pre></td></tr>
	<tr><th>angular.isString</th><td><pre>angular.isString({value})</pre></td></tr>
	<tr><th>angular.isUndefined</th><td><pre>angular.isUndefined({value})</pre></td></tr>
	<tr><th>angular.lowercase</th><td><pre>angular.lowercase({string})</pre></td></tr>
	<tr><th>angular.module</th><td><pre>angular.module('{moduleName}', [|])</pre></td></tr>
	<tr><th>angular.noop</th><td><pre>angular.noop</pre></td></tr>
	<tr><th>angular.toJson</th><td><pre>angular.toJson({string})</pre></td></tr>
	<tr><th>angular.uppercase</th><td><pre>angular.uppercase({string})</pre></td></tr>
	<tr><th>angular.version</th><td><pre>angular.version</pre></td></tr>
</table>

## Services

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>config</th><td><pre>config([function() {
	|
}])</pre></td></tr>
	<tr><th>constant</th><td><pre>constant('{name}', {value})</pre></td></tr>
	<tr><th>controller</th><td><pre>controller('{Name}Ctrl', [function({$scope}) {
	|
}])</pre></td></tr>
	<tr><th>decorator</th><td><pre>decorator('{name}', [function($provide) {
	$provide.decorator('{name}', [function($delegate) {
		return {$delegate}|;
	}]);
}])</pre></td></tr>
	<tr><th>directive</th><td><pre>directive('{name}', [function {name}Factory() {
	return {
		restrict: '{A}',
		link(scope, iElement, iAttrs) {
			|
		}
	};
}])</pre></td></tr>
	<tr><th>directivelong</th><td><pre>directive('{name}', [function {name}Factory() {
	return {|
		priority: 0,
		template: '&lt;div&gt;&lt;/div&gt;',
		templateUrl: 'directive.html',
		replace: true,
		transclude: true,
		restrict: 'A',
		scope: {},
		controller: function($scope, $element, $attrs, $transclude, otherInjectables) {

		},
		compile: function compile(tElement, tAttrs, transclude) {
			return function postLink(scope, iElement, iAttrs, controller) {

			}
		},
		link: function postLink(scope, iElement, iAttrs) {

		}
	};
}])</pre></td></tr>
	<tr><th>factory</th><td><pre>factory('{name}', [function {name}Get() {
	|

	return {

	};
}])</pre></td></tr>
	<tr><th>provider</th><td><pre>provider('{name}', [function {name}Constructor() {
	|

	this.$get = [function() {
		return {

		};
	}];
}])</pre></td></tr>
	<tr><th>run</th><td><pre>run([function() {
	|
}])</pre></td></tr>
	<tr><th>service</th><td><pre>service('{name}', [function {name}Constructor() {
	|
}])</pre></td></tr>
	<tr><th>value</th><td><pre>value('{name}', {value})</pre></td></tr>
</table>

## Variables

- angular
- anchorScroll
- animation
- animator
- cacheFactory
- compile
- controller
- exceptionHandler
- location
- locationProvider
- log
- parse
- resource
- rootElement
- rootScope
- route
- routeParams
- routeProvider
- templateCache
- timeout
- scope

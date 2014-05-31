# Angular.js Snippets for Sublime Text

This snippet library provides completions for Angular.js’s stable and unstable branch.
Sublime Text uses fuzzy searching for snippets and completions therefore you don’t have to write triggers completely.
All snippets add Angular’s inline notation for dependencies automatically, so you don’t have to type them twice.

## Installation

- Package Control: install the package "AngularJS Snippets"
- Manual: copy files to your Sublime Text User folder

## IMPORTANT

Completions won’t show in HTML unless you have added this line to your User.sublime-preferences:

	"auto_complete_triggers": [ {"selector": "text.html", "characters": "<"}, {"selector": "text.html meta.tag", "characters": " " } ]

__Snippet Categories:__
- [Services](#services)
- [Directives](#directives)
- [Globals](#globals)
- [jQuery lite](#jquery-lite)
- [Scope functions](#scope-functions)
- [Log functions](#log-functions)
- [Variables](#variables)

## Services

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>config</th><td><pre>config([function() {
	|
}])</pre></td></tr>
	<tr><th>constant</th><td><pre>constant('{name}', {value})</pre></td></tr>
	<tr><th>controller</th><td><pre>controller('{Name}Ctrl', [function ({$scope}) {
	|
}])</pre></td></tr>
	<tr><th>decorator</th><td><pre>decorator('{name}', [function ($provide) {
	$provide.decorator('{name}', [function($delegate) {
		return {$delegate}|;
	}]);
}])</pre></td></tr>
	<tr><th>directive</th><td><pre>directive('{name}', [function () {
	return {
		restrict: '{A}',
		link: function(scope, iElement, iAttrs) {
			|
		}
	};
}])</pre></td></tr>
	<tr><th>directivelong</th><td><pre>directive('{name}', [function () {
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
	<tr><th>factory</th><td><pre>factory('{name}', [function () {
	|

	return {

	};
}])</pre></td></tr>
	<tr><th>otherwise</th><td><pre>otherwise({ redirectTo: '/{route}' })</pre></td></tr>
	<tr><th>provider</th><td><pre>provider('{name}', [function () {
	|

	this.$get = [function() {
		return {

		};
	}];
}])</pre></td></tr>
	<tr><th>run</th><td><pre>run([function() {
	|
}])</pre></td></tr>
	<tr><th>service</th><td><pre>service('{name}', [function () {
	|
}])</pre></td></tr>
	<tr><th>value</th><td><pre>value('{name}', {value})</pre></td></tr>
	<tr><th>when</th><td><pre>when('/{name}', {
	templateUrl: '{name}.html',
	controller: '{Name}Ctrl'
})</pre></td></tr>
</table>

## Directives

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>ng-animate</th><td>ng-animate="{enter: '{example}-enter', leave: '{example}-leave'}"</td></tr>
	<tr><th>ng-animates</th><td>ng-animate="'{class-prefix}'"</td></tr>
	<tr><th>ng-app</th><td>ng-app=""</td></tr>
	<tr><th>ng-bind</th><td>ng-bind=""</td></tr>
	<tr><th>ng-bind-html-unsafe</th><td>ng-bind-html-unsafe=""</td></tr>
	<tr><th>ng-bind-template</th><td>ng-bind-template=""</td></tr>
	<tr><th>ng-change</th><td>ng-change=""</td></tr>
	<tr><th>ng-checked</th><td>ng-checked=""</td></tr>
	<tr><th>ng-class</th><td>ng-class=""</td></tr>
	<tr><th>ng-class-even</th><td>ng-class-even=""</td></tr>
	<tr><th>ng-class-odd</th><td>ng-class-odd=""</td></tr>
	<tr><th>ng-click</th><td>ng-click=""</td></tr>
	<tr><th>ng-cloak</th><td>ng-cloak</td></tr>
	<tr><th>ng-controller</th><td>ng-controller="{Name}Ctrl"</td></tr>
	<tr><th>ng-dblclick</th><td>ng-dblclick=""</td></tr>
	<tr><th>ng-disabled</th><td>ng-disabled=""</td></tr>
	<tr><th>ng-form</th><td>ng-form=""</td></tr>
	<tr><th>ng-hide</th><td>ng-hide=""</td></tr>
	<tr><th>ng-href</th><td>ng-href=""</td></tr>
	<tr><th>ng-if</th><td>ng-if=""</td></tr>
	<tr><th>ng-include</th><td>ng-include="{template}" {onload="" autoscroll=""}</td></tr>
	<tr><th>ng-init</th><td>ng-init=""</td></tr>
	<tr><th>ng-keydown</th><td>ng-keydown=""</td></tr>
	<tr><th>ng-keypress</th><td>ng-keypress=""</td></tr>
	<tr><th>ng-keyup</th><td>ng-keyup=""</td></tr>
	<tr><th>ng-list</th><td>ng-list=""</td></tr>
	<tr><th>ng-model</th><td>ng-model=""</td></tr>
	<tr><th>ng-mousedown</th><td>ng-mousedown=""</td></tr>
	<tr><th>ng-mouseenter</th><td>ng-mouseenter=""</td></tr>
	<tr><th>ng-mouseleave</th><td>ng-mouseleave=""</td></tr>
	<tr><th>ng-mousemove</th><td>ng-mousemove=""</td></tr>
	<tr><th>ng-mouseover</th><td>ng-mouseover=""</td></tr>
	<tr><th>ng-mouseup</th><td>ng-mouseup=""</td></tr>
	<tr><th>ng-multiple</th><td>ng-multiple=""</td></tr>
	<tr><th>ng-nbind</th><td>ng-non-bindable=""</td></tr>
	<tr><th>ng-open</th><td>ng-open=""</td></tr>
	<tr><th>ng-pluralize</th><td>ng-pluralize count="" when="'': '{}'"</td></tr>
	<tr><th>ng-readonly</th><td>ng-readonly=""</td></tr>
	<tr><th>ng-repeat</th><td>ng-repeat="{item} in {array}"</td></tr>
	<tr><th>ng-selected</th><td>ng-selected=""</td></tr>
	<tr><th>ng-show</th><td>ng-show=""</td></tr>
	<tr><th>ng-src</th><td>ng-src=""</td></tr>
	<tr><th>ng-style</th><td>ng-style=""</td></tr>
	<tr><th>ng-submit</th><td>ng-submit=""</td></tr>
	<tr><th>ng-swipe-left</th><td>ng-swipe-left=""</td></tr>
	<tr><th>ng-swipe-right</th><td>ng-swipe-right=""</td></tr>
	<tr><th>ng-switch</th><td>ng-switch on=""</td></tr>
	<tr><th>ng-switch-default</th><td>ng-switch-default=""</td></tr>
	<tr><th>ng-switch-when</th><td>ng-switch-when=""</td></tr>
	<tr><th>ng-transclude</th><td>ng-transclude</td></tr>
	<tr><th>ng-view</th><td>ng-view</td></tr>
</table>

## Globals

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular.bind</th><td><pre>angular.bind({self}, {function})</pre></td></tr>
	<tr><th>angular.bootstrap</th><td><pre>angular.bootstrap({element}{, [{modules}]})</pre></td></tr>
	<tr><th>angular.copy</th><td><pre>angular.copy({source}{, {destination}})</pre></td></tr>
	<tr><th>angular.element</th><td><pre>angular.element({element})</pre></td></tr>
	<tr><th>angular.equals</th><td><pre>angular.equals({obj1}, {obj2})</pre></td></tr>
	<tr><th>angular.extend</th><td><pre>angular.extend({destination}, {source})</pre></td></tr>
	<tr><th>angular.forEach</th><td><pre>angular.forEach({obj}, {iterator})</pre></td></tr>
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
	<tr><th>angular.module</th><td><pre>angular.module('{moduleName}', [])</pre></td></tr>
	<tr><th>angular.noop</th><td><pre>angular.noop</pre></td></tr>
	<tr><th>angular.toJson</th><td><pre>angular.toJson({string})</pre></td></tr>
	<tr><th>angular.uppercase</th><td><pre>angular.uppercase({string})</pre></td></tr>
	<tr><th>angular.version</th><td><pre>angular.version</pre></td></tr>
</table>

## jQuery lite

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular: addClass</th><td><pre>addClass({className})</pre></td></tr>
	<tr><th>angular: after</th><td><pre>after({el})</pre></td></tr>
	<tr><th>angular: append</th><td><pre>append({el})</pre></td></tr>
	<tr><th>angular: attr</th><td><pre>attr({el})</pre></td></tr>
	<tr><th>angular: bind</th><td><pre>bind({eventType}{, eventData}{, eventHandler})</pre></td></tr>
	<tr><th>angular: children</th><td><pre>children()</pre></td></tr>
	<tr><th>angular: clone</th><td><pre>clone({withDataAndEvents})</pre></td></tr>
	<tr><th>angular: contents</th><td><pre>contents({withDataAndEvents})</pre></td></tr>
	<tr><th>angular: css</th><td><pre>css({propertyName(s)})</pre></td></tr>
	<tr><th>angular: data</th><td><pre>data({key, value | obj})</pre></td></tr>
	<tr><th>angular: eq</th><td><pre>eq({index})</pre></td></tr>
	<tr><th>angular: find</th><td><pre>find({tag})</pre></td></tr>
	<tr><th>angular: hasClass</th><td><pre>hasClass({className})</pre></td></tr>
	<tr><th>angular: html</th><td><pre>html()</pre></td></tr>
	<tr><th>angular: next</th><td><pre>next()</pre></td></tr>
	<tr><th>angular: parent</th><td><pre>parent()</pre></td></tr>
	<tr><th>angular: prepend</th><td><pre>prepend({content})</pre></td></tr>
	<tr><th>angular: prop</th><td><pre>prop({propertyName})</pre></td></tr>
	<tr><th>angular: ready</th><td><pre>ready({handler})</pre></td></tr>
	<tr><th>angular: remove</th><td><pre>remove({selector})</pre></td></tr>
	<tr><th>angular: removeAttr</th><td><pre>removeAttr({attributeName})</pre></td></tr>
	<tr><th>angular: removeClass</th><td><pre>removeClass({className})</pre></td></tr>
	<tr><th>angular: removeData</th><td><pre>removeData({name})</pre></td></tr>
	<tr><th>angular: replaceWith</th><td><pre>replaceWith({newContent})</pre></td></tr>
	<tr><th>angular: text</th><td><pre>text()</pre></td></tr>
	<tr><th>angular: toggleClass</th><td><pre>toggleClass({className})</pre></td></tr>
	<tr><th>angular: triggerHandler</th><td><pre>triggerHandler({eventType})</pre></td></tr>
	<tr><th>angular: unbind</th><td><pre>unbind({eventType{, handler})</pre></td></tr>
	<tr><th>angular: val</th><td><pre>val({eventType{, handler})</pre></td></tr>
	<tr><th>angular: wrap</th><td><pre>wrap({wrappingElement})</pre></td></tr>

	<tr><th>angular: controller</th><td><pre>controller({name})</pre></td></tr>
	<tr><th>angular: injector</th><td><pre>injector()</pre></td></tr>
	<tr><th>angular: scope</th><td><pre>scope()</pre></td></tr>
	<tr><th>angular: inheritedData</th><td><pre>inheritedData()</pre></td></tr>
</table>

## Scope functions

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular: $apply</th><td><pre>apply({exp})</pre></td></tr>
	<tr><th>angular: $broadcast</th><td><pre>broadcast({name}{, args})</pre></td></tr>
	<tr><th>angular: $destroy</th><td><pre>destroy()</pre></td></tr>
	<tr><th>angular: $digest</th><td><pre>digest()</pre></td></tr>
	<tr><th>angular: $emit</th><td><pre>emit({name}{, args})</pre></td></tr>
	<tr><th>angular: $eval</th><td><pre>eval({expression})</pre></td></tr>
	<tr><th>angular: $evalAsync</th><td><pre>evalAsync({expression})</pre></td></tr>
	<tr><th>angular: $new</th><td><pre>new({isolate})</pre></td></tr>
	<tr><th>angular: $on</th><td><pre>on({name}, {listener})</pre></td></tr>
	<tr><th>angular: $watch</th><td><pre>watch({watchExpression}{, listener}{, objectEquality})</pre></td></tr>
	<tr><th>angular: $watchCollection</th><td><pre>watchCollection({obj}, {listener})</pre></td></tr>
	<tr><th>angular: $id</th><td><pre>id</pre></td></tr>
</table>

# Log functions

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular: $log.debug</th><td><pre>log.debug('{debug}')</pre></td></tr>
	<tr><th>angular: $log.error</th><td><pre>log.error('{error}')</pre></td></tr>
	<tr><th>angular: $log.info</th><td><pre>log.info('{info}')</pre></td></tr>
	<tr><th>angular: $log.log</th><td><pre>log.log('{log}')</pre></td></tr>
	<tr><th>angular: $log.warn</th><td><pre>log.warn('{warning}')</pre></td></tr>
	<tr><th>angular: $log.assertEmpty</th><td><pre>log.assertEmpty()</pre></td></tr>
	<tr><th>angular: $log.reset</th><td><pre>log.reset()</pre></td></tr>
</table>

## Variables

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>angular: $angular</th><td><pre>angular</pre></td></tr>
	<tr><th>angular: $anchorScroll</th><td><pre>anchorScroll</pre></td></tr>
	<tr><th>angular: $animation</th><td><pre>animation</pre></td></tr>
	<tr><th>angular: $animator</th><td><pre>animator</pre></td></tr>
	<tr><th>angular: $cacheFactory</th><td><pre>cacheFactory</pre></td></tr>
	<tr><th>angular: $compile</th><td><pre>compile</pre></td></tr>
	<tr><th>angular: $controller</th><td><pre>controller</pre></td></tr>
	<tr><th>angular: $exceptionHandler</th><td><pre>exceptionHandler</pre></td></tr>
	<tr><th>angular: $location</th><td><pre>location</pre></td></tr>
	<tr><th>angular: $locationProvider</th><td><pre>locationProvider</pre></td></tr>
	<tr><th>angular: $log</th><td><pre>log</pre></td></tr>
	<tr><th>angular: $parse</th><td><pre>parse</pre></td></tr>
	<tr><th>angular: $resource</th><td><pre>resource</pre></td></tr>
	<tr><th>angular: $rootElement</th><td><pre>rootElement</pre></td></tr>
	<tr><th>angular: $rootScope</th><td><pre>rootScope</pre></td></tr>
	<tr><th>angular: $route</th><td><pre>route</pre></td></tr>
	<tr><th>angular: $routeParams</th><td><pre>routeParams</pre></td></tr>
	<tr><th>angular: $routeProvider</th><td><pre>routeProvider</pre></td></tr>
	<tr><th>angular: $templateCache</th><td><pre>templateCache</pre></td></tr>
	<tr><th>angular: $timeout</th><td><pre>timeout</pre></td></tr>
	<tr><th>angular: $scope</th><td><pre>scope</pre></td></tr>
</table>

## LICENSE

The MIT License (MIT)

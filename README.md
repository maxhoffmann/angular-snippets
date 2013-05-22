# Angular.js Snippets for Sublime Text 2

## Installation

- Package Control: install the package "AngularJS Snippets"
- Manual: copy files to the Sublime packages folder

## Directives (HTML attributes)

html standard attributes are suffixed with `a`, e.g. `classa`

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>app</th><td>ng-app="|"</td></tr>
	<tr><th>bind</th><td>ng-bind="|"</td></tr>
	<tr><th>bindh</th><td>ng-bind-html-unsafe="|"</td></tr>
	<tr><th>bindt</th><td>ng-bind-template="|"</td></tr>
	<tr><th>change</th><td>ng-change="|"</td></tr>
	<tr><th>checked<span style="color: green">a</span></th><td>ng-checked="|"</td></tr>
	<tr><th>class<span style="color: green">a</span></th><td>ng-class="|"</td></tr>
	<tr><th>classe</th><td>ng-class-even="|"</td></tr>
	<tr><th>classo</th><td>ng-class-odd="|"</td></tr>
	<tr><th>click</th><td>ng-click="|"</td></tr>
	<tr><th>cloak</th><td>ng-cloak</td></tr>
	<tr><th>ctrl, controller</th><td>ng-controller="{Name}Ctrl"</td></tr>
	<tr><th>dclick</th><td>ng-dblclick="|"</td></tr>
	<tr><th>disabled<span style="color: green">a</span></th><td>ng-disabled="|"</td></tr>
	<tr><th>form<span style="color: green">a</span></th><td>ng-form="|"</td></tr>
	<tr><th>hide</th><td>ng-hide="|"</td></tr>
	<tr><th>href<span style="color: green">a</span></th><td>ng-href="|"</td></tr>
	<tr><th>include</th><td>ng-include="{template}" {onload="|" autoscroll="|"}</td></tr>
	<tr><th>init</th><td>ng-init="|"</td></tr>
	<tr><th>list</th><td>ng-list="|"</td></tr>
	<tr><th>model</th><td>ng-model="|"</td></tr>
	<tr><th>mousedown</th><td>ng-mousedown="|"</td></tr>
	<tr><th>mouseenter</th><td>ng-mouseenter="|"</td></tr>
	<tr><th>mouseleave</th><td>ng-mouseleave="|"</td></tr>
	<tr><th>mousemove</th><td>ng-mousemove="|"</td></tr>
	<tr><th>mouseover</th><td>ng-mouseover="|"</td></tr>
	<tr><th>mouseup</th><td>ng-mouseup="|"</td></tr>
	<tr><th>multiple</th><td>ng-multiple="|"</td></tr>
	<tr><th>nbind</th><td>ng-non-bindable="|"</td></tr>
	<tr><th>pluralize</th><td>&lt;ng-pluralize count="|" when="'|': '{}'"&gt;&lt;/ng-pluralize&gt;</td></tr>
	<tr><th>readonly<span style="color: green">a</span></th><td>ng-readonly="|"</td></tr>
	<tr><th>repeat</th><td>ng-repeat="{item} in {array}"</td></tr>
	<tr><th>selected<span style="color: green">a</span></th><td>ng-selected="|"</td></tr>
	<tr><th>show</th><td>ng-show="|"</td></tr>
	<tr><th>src<span style="color: green">a</span></th><td>ng-src="|"</td></tr>
	<tr><th>style<span style="color: green">a</span></th><td>ng-style="|"</td></tr>
	<tr><th>submit</th><td>ng-submit="|"</td></tr>
	<tr><th>switch</th><td>ng-switch="|" on="|"</td></tr>
	<tr><th>switchd</th><td>ng-switch-default="|"</td></tr>
	<tr><th>switchw</th><td>ng-switch-when="|"</td></tr>
	<tr><th>trans, transclude</th><td>ng-transclude</td></tr>
	<tr><th>view</th><td>ng-view</td></tr>
</table>

## JavaScript

### Globals


<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>abind</th><td><pre>angular.bind({self}, {function}|)</pre></td></tr>
	<tr><th>abootstrap</th><td><pre>angular.bootstrap({element}{, [{modules}]})</pre></td></tr>
	<tr><th>acopy</th><td><pre>angular.copy({source}{, {destination}})</pre></td></tr>
	<tr><th>aelement</th><td><pre>angular.element({element})</pre></td></tr>
	<tr><th>aequals</th><td><pre>angular.equals({obj1}, {obj2})</pre></td></tr>
	<tr><th>abind</th><td><pre>angular.extend({destination}, {source})</pre></td></tr>
	<tr><th>abind</th><td><pre>angular.forEach({obj}, {iterator}|)</pre></td></tr>
	<tr><th>abind</th><td><pre>angular.fromJson({jsonString})</pre></td></tr>
	<tr><th>abind</th><td><pre>angular.identity()</pre></td></tr>
	<tr><th>abind</th><td><pre>angular.injector([{modules}])</pre></td></tr>
	<tr><th>aisarray</th><td><pre>angular.isArray({value})</pre></td></tr>
	<tr><th>aisdate</th><td><pre>angular.isDate({value})</pre></td></tr>
	<tr><th>aisdefined</th><td><pre>angular.isDefined({value})</pre></td></tr>
	<tr><th>aiselement</th><td><pre>angular.isElement({value})</pre></td></tr>
	<tr><th>aisfunction</th><td><pre>angular.isFunction({value})</pre></td></tr>
	<tr><th>aisnumber</th><td><pre>angular.isNumber({value})</pre></td></tr>
	<tr><th>aisobject</th><td><pre>angular.isObject({value})</pre></td></tr>
	<tr><th>aisstring</th><td><pre>angular.isString({value})</pre></td></tr>
	<tr><th>aisundefined</th><td><pre>angular.isUndefined({value})</pre></td></tr>
	<tr><th>alowercase</th><td><pre>angular.lowercase({string})</pre></td></tr>
	<tr><th>amodule</th><td><pre>angular.module('{moduleName}', [|])</pre></td></tr>
	<tr><th>anoop</th><td><pre>angular.noop</pre></td></tr>
	<tr><th>atojson</th><td><pre>angular.toJson({string})</pre></td></tr>
	<tr><th>auppercase</th><td><pre>angular.uppercase({string})</pre></td></tr>
	<tr><th>aversion</th><td><pre>angular.version</pre></td></tr>
</table>

### Services & Types

<table>
	<tr><th>trigger</th><th>completion</th></tr>
	<tr><th>config</th><td><pre>config(function(|) {
	|
});</pre></td></tr>
	<tr><th>constant</th><td><pre>constant('{name}', {value});</pre></td></tr>
	<tr><th>ctrl, controller</th><td><pre>controller('{Name}Ctrl', function({$scope}) {
	|
});</pre></td></tr>
	<tr><th>decorator</th><td><pre>decorator('{name}', function($provide) {
	$provide.decorator('{name}', function($delegate) {
		return {$delegate}|;
	});
});</pre></td></tr>
	<tr><th>directive</th><td><pre>directive('{name}', function {name}Factory(|) {
  return {
	restrict: '{A}',
	link(scope, iElement, iAttrs) {
		|
	}
  };
});</pre></td></tr>
	<tr><th>factory</th><td><pre>factory('{name}', function {name}Get(|) {
	|

	return {

	};
});</pre></td></tr>
	<tr><th>provider</th><td><pre>provider('{name}', function {name}Constructor(|) {
	|

	this.$get = function() {
		return {

		};
	};
});</pre></td></tr>
	<tr><th>run</th><td><pre>run(function(|) {
	|
});</pre></td></tr>
	<tr><th>service</th><td><pre>service('{name}', function {name}Constructor(|) {
	|
});</pre></td></tr>
	<tr><th>value</th><td><pre>value('{name}', {value});</pre></td></tr>
</table>
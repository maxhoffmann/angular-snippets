# Angular.js Snippets for Sublime Text 2

## Installation

- Package Control: install the package "Angular.js Snippets"
- Manual: copy files to the Sublime packages folder

## HTML Snippets

default attributes are suffixed with `a`, e.g. `classa`

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
	<tr><th>switch</th><td>ng-switch="|"</td></tr>
	<tr><th>switchd</th><td>ng-switch-default="|" on="|"</td></tr>
	<tr><th>switchw</th><td>ng-switch-when="|"</td></tr>
	<tr><th>transclude</th><td>ng-transclude</td></tr>
	<tr><th>view</th><td>ng-view</td></tr>
</table>

## JavaScript Snippets

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
	<tr><th>module</th><td><pre>angular.module('{moduleName}', [|]);</pre></td></tr>
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
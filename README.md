# Angular2 [innerContent] directive
An Angular2 directive to parse string contents and render the directive contents inside it.

This directive works as [htmlContent] but instead of simple HTML it proccess directives too.

The @Input innerContent receives an array argument, the first array element
is the code to be parsed. The second index is an array of Components that
contains the directives present in the code.

Example:

<div [innerContent]="[
	'Go to <a [routerLink]="[Home]">Home page</a>',
	[RouterLink]
]">


# snm-accordion-group
This is an addon for html accordions used in SNM Web Applications. This outlines the details of collaborating on this Ember addon.

## Consumption
Make sure the npm registry is set to ASH's private registry. 
Execute below commands from the consuming application root terminal. 

  * ***ember install snm-accordion-group***
  * ***ember generate snm-accordion-group***


## Usage in the templates
**Accordion Group:**
```

    {{#snm-accordion-group title="Member Info" autoExpand="true" as |accordionGroup|}}
        {{#accordionGroup.accordion  title="Elig Info" classNames="max"}}
            <div class="panel-body">Content for the first Accordion in the group!</div>
        {{/accordionGroup.accordion}}

        {{#accordionGroup.accordion title="Ihis Info" classNames="max"}}
            <div>Content for the second Accordion in the group!</div>
        {{/accordionGroup.accordion}}

        {{#accordionGroup.accordion title="Claim Info" }}
            <div>Content for the third Accordion in the group!</div>
        {{/accordionGroup.accordion}}
    {{/snm-accordion-group}} 
```
**Standalone Accordion:**
```
    {{#snm-accordion title="Member Summary" classNames="standard"}}
        <div class="panel-body">Content for the snm-accordion</div>
    {{/snm-accordion}}
```

## Options 

 ### title
   Title for the accordion.
   
 ### enableToggle
   Flag for the toggle feature. Defaults to `true`
   
 ### autoExpand 
   Flag for the accordion to be expanded when initially loaded. Defaults to `true`
   
 ### classNames 
 Sets the size of the accordion through css classes. Defaults to `full`

**Alternate options:**
  
  `full` (99% of the screen/container)  

  `max` (97% of the screen/container) 

  `standard` (90% of the screen/container) 

  `min-x-3` (75% of the screen/container) 

  `min-x-2` (50% of the screen/container) 

  `min` (25% of the screen/container) 

## Dependency
This addon has some dependency on Bootstrap 3.3.7 and Fontawesome 4.7.0 and will inherit the bootstrap styles used by the consuming application. 

## Development Installation

* `git clone <repository-url>` this repository
* `cd snm-accordion-group`
* `npm install`
* `bower install`

## Running

* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).

## Running Tests

* `npm test` (Runs `ember try:each` to test your addon against multiple Ember versions)
* `ember test`
* `ember test --server`

## Building

* `ember build`

For more information on using ember-cli, visit [https://ember-cli.com/](https://ember-cli.com/).


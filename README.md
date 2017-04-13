[![Ember Observer Score](http://emberobserver.com/badges/ember-browser-checker.svg)](http://emberobserver.com/addons/ember-browser-checker)

### Ember-browser-checker

### Installation

-------------

`ember install ember-browser-checker`

### Usage

-------------

Check what browser is being used with ease. For example:

+ Print a special message for safari:

```
{{#if (is-safari)}}
  I'm on a safari!
{{/if}}
```

+ Get the name of the user's brower:

```
You are on {{browser-name}}.
```

+ Inject the `browserChecker` service and use everywhere else

```js
browserChecker: Ember.inject.service();
...
this.get('browserChecker').get('isChrome')
```

---------

#### Browser Support

Name     | Helper
---------|-----------
Blink    | `is-blink`
Chrome   | `is-chrome`
Edge     | `is-edge`
Explorer | `is-explorer`
Firefox  | `is-firefox`
Opera    | `is-opera`
Safari   | `is-safari`

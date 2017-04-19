# terms-transformer

A Polymer Element that is used to convert a list of selected ids from the `<feature-aggregation>`
component to an object structure to use with `<selected-facets-display>`, and vice versa.

```html
    <terms-transformer
      category="[[title]]"
      list="{{selectedList}}"
      object="{{searchParamSubset}}">
    </terms-transformer>
```

### Dependencies

Dependencies are installed using [Bower](http://bower.io/):

    npm install -g bower
    bower install

### Testing

Tests are run using [web-component-tester](https://github.com/Polymer/web-component-tester):

    npm install -g web-component-tester
    wct

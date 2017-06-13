# terms-transformer

A Polymer Element that is used to convert a list of selected ids from the `<feature-aggregation>`
component to an object structure to use with `<selected-facets-display>`, and vice versa.

### Example without object property
```js
var selectedList = ['one', 'two'];
var selectedObject = {
  one: {
    category: 'Category',
    enabled: true,
    id: 'one',
    text: 'One'
  },
  two: {
    category: 'Category',
    enabled: true,
    id: 'two',
    text: 'Two'
  }
};
```

```html
<terms-transformer
  category="Category"
  list="{{selectedList}}"
  object="{{selectedObject}}">
</terms-transformer>
```

### Example with object property
```js
var selectedList = ['one', 'two'];
var selectedObject = {
  property: {
    one: {
      category: 'Category',
      enabled: true,
      id: 'one',
      text: 'One'
    },
    two: {
      category: 'Category',
      enabled: true,
      id: 'two',
      text: 'Two'
    }
  }
};
```

```html
<terms-transformer
  category="Category"
  object-property="property"
  list="{{selectedList}}"
  object="{{selectedObject}}">
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

### Demonstration & Documentation

Demonstration and documentation are viewed using [polyserve](https://github.com/PolymerLabs/polyserve):

    npm install -g polyserve
    polyserve

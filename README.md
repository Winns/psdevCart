## psdev.cart.js

### Description
JavaScript tiny cart script, with multitab sync.

### Require
jQuery

### Cart creation options
Name         | Type                            | Description
-------------|---------------------------------|-------------
syncInterval | Integer                         | localStorage sync interval
constructor  | Function                        | Contructor function
elAdd        | String                          | Class for item add button
elRemove     | String                          | Class for item remove button
elPlus       | String                          | Class for item add or +1 button
elMinus      | String                          | Class for item remove or -1 button, you can use data-limit="1" to disable item remove when count < 1
elCountInput | String                          | Class for count input

### myCart.on() method

#### render - trigger when cart need to be rendered
``` js
myCart.on('render', function(data) {
    /*
    data = {
            updateTime: - last update time,
            count: number of cart items,
            items: cart items
    };
   */
});
```

#### add - trigger on item add
``` js
myCart.on('add', function(data) {
    // data = { id: id, count: 1 };
});
```

#### remove - trigger on item remove
``` js
myCart.on('remove', function(itemId) {

});
```

#### clear - trigger on cart clear
``` js
myCart.on('clear', function() {

});
```

#### save - trigger on cart save
``` js
myCart.on('save', function(data) {
    /*
    data = {
            updateTime: - last update time,
            count: number of cart items,
            items: cart items
    };
   */
});
```

### Demo
[Link](http://winns.github.io/psdevCart-demo-page/)

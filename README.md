# This is my repository

### My name is CAT

![CAT](https://cdn.omlet.com/images/cache/850/567/breed_abyssinian_cat.webp)

**I am JavaScript developer** 
*It`s my code example*

```javascript
let orderForm = document.getElementById('order-form');
let orderTable = document.getElementById('order-table');
let orders = [];

orderForm.addEventListener('submit', function(event) {
    // stop form submission
    event.preventDefault();

    let order = {
        dish: event.target['dish'].value,
        time: event.target['time'].value,
        address: event.target['address'].value,
        tel: event.target['tel'].value
    }
    event.target.reset();

    const serializer = new XMLSerializer();
    const xmlStr = serializer.serializeToString(event.target);
    console.log(xmlStr);
    orders.push(order);
    drawOrder(order);
});
```

This is unordered list
 * [First](http://goolge.com)
 * [Second](http://github.com)



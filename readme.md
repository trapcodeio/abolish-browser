## Abolish for browser

To use [abolish](https://www.npmjs.com/package/abolish) directly in your browser without package managers.


### From CDN
```html
<script src="https://cdn.jsdelivr.net/npm/abolish-browser/abolish.min.js"></script>
```
`Abolish` is exposed as `window.Abolish` while
`Rule` is exposed as `window.AbolishRule`
`ParseRules` is exposed as `window.AbolishParseRules`

```html
<script>
    const form = {
        age: 10
    };

    const rules = {
        age: 'max:5'
    };

    console.log(Abolish.validate(form, rules))
</script>
```

```json
{
  "error": {
    "key": "age",
    "type": "validator",
    "validator": "max",
    "message": "Age is too big. (Max. 5)",
    "data": null
  }
}
```
visit [abolish documentation](https://www.npmjs.com/package/abolish)


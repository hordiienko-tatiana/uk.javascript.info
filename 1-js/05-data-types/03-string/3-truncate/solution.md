Максимальна довжина має бути `maxlength`, тому нам потрібно її трохи обрізати, щоб дати місце для символу трьох крапок.

Зауважте, що насправді існує один юнікодний символ для "трьох крапок". Це не три послідовні крапки.

```js run demo
function truncate(str, maxlength) {
  return (str.length > maxlength) ?
    str.slice(0, maxlength - 1) + '…' : str;
}
```

🛠 В коде можно смешивать использование обоих видов строк: использовать обычные строки для статических значений, а для динамических – шаблонные строки.

🛠 Шаблонные строки могут быть очень полезны для формирования динамической html-разметки с помощью JavaScript.

```js
const inner = `
<form>
  <input type="text" />
  <button>Submit</button>
</form>
`;

const errorText = `Внимание! Ваш аккаут <b>${accountName}</b> заблокирован.`;
```

::: callout ❗️

Будьте осторожны при написании html внутри шаблонных строк. Шаблонные строки, так же как и обычные, не экранируют спецсимволы. Это значит что использование ненадёжного html из шаблонной строки может привести к различным [атакам](/js/web-security).

:::

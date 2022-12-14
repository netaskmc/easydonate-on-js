# easydonate-on-js
### Неофициальная API-обёртка для easydonate.ru на JavaScript (Модуль ES6).

Основано на `node-fetch` API.

Эта библиотека нестабильна! Используйте её на свой страх и риск! Однако, мы следуем SemVer, поэтому вы можете быть уверены, что API не внесёт обратно несовместимые изменения без бампа мажорной версии (1.\*.\* > 2.\*.\*).

Если вы встретили проблемы при использовании этой библиотеки, пожалуйста, не беспокойте EasyDonate, вместо этого создайте issue в этом репозитории.

⚠ ***Примечание:** Эта библиотека не предназначена для использования на фронтенде (в браузере)! Вы **ОТКРОЕТЕ ДОСТУП к ключу магазина** третьим лицам.*

## Использование
```
$ npm install easydonate-on-js
```

```javascript
// ES6
import { EasyDonate } from 'easydonate-on-js';

const shopKey = 'abcde123abcde123abcde123abcde123'; // Ваш ключ магазина
const easyDonate = new EasyDonate(shopKey);

// Получение информации о магазине
let shopInfo = await easyDonate.shop();
console.log(shopInfo.name); // Выведет название магазина
```

[English README](README.md)
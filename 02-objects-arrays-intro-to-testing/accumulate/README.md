# accumulate

Необходимо реализовать функцию, которая преобразует массив объектов в единый объект.
Функция принимает первый аргумент `config` - массива строк. Это те свойства которые мы будем искать в массиве с данными.
И второй аргумент `data` - массива объектов, внутри которых мы будем искать значения и аккумулировать 
(собирать в соответствующие свойства) в результирующем объекте.

**Пример:**
```javascript
const config = [
  'price',
  'sales'
];

const data = [
  {
    title: "Соска (пустышка) NUK 10729357",
    price: 3,
    sales: 0
  },
  {
    title: "ТВ тюнер D-COLOR  DC1301HD",
    price: 15,
    sales: 13
  },
  {
    title: "Детский велосипед Lexus Trike Racer Trike",
    price: 53,
    sales: 11
  },
];

accumulate(config, data);

// Результат:
// const result = {
//   price: [3, 15, 53],
//   sales: [0, 13, 11]
// }
```
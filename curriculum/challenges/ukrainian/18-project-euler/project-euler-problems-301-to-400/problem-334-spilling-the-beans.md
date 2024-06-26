---
id: 5900f4ba1000cf542c50ffcd
title: 'Завдання 334: розсипання бобів'
challengeType: 1
forumTopicId: 301992
dashedName: problem-334-spilling-the-beans
---

# --description--

В раю Платона існує нескінченна кількість мисок, які стоять в прямій лінії. Кожна миска або містить скінченну кількість бобів, або ні. Дитина грає гру, де можна ходити лише одним способом: забрати два боби з будь-якої миски, і покласти по одному в сусідні дві миски. Гра закінчується, коли у кожній мисці є хоча б один біб або немає жодного.

Наприклад, у двох сусідніх мисках лежать 2 і 3 боби відповідно, а всі інші миски — пусті. Наступні 8 кроків завершать гру:

<img alt="анімація гри, де у двох сусідніх мисках є 2 і 3 боби відповідно" src="https://cdn.freecodecamp.org/curriculum/project-euler/spilling-the-beans.gif" style="background-color: white; padding: 10px; display: block; margin-right: auto; margin-left: auto; margin-bottom: 1.2rem;" />

Дано такі послідовності:

$$\begin{align}   & t_0 = 123456, \\\\
  & t_i = \begin{cases}          \frac{t_{i - 1}}{2},               & \text{якщо $t_{i - 1}$ парне} \\\\
         \left\lfloor\frac{t_{i - 1}}{2}\right\rfloor \oplus 926252, & \text{якщо $t_{i - 1}$ непарне}          \end{cases} \\\\
         & \qquad \text{де $⌊x⌋$ є функцією підлоги, а $\oplus$ є бітовим оператором XOR.} \\\\ & b_i = (t_i\bmod 2^{11}) + 1. \end{align}$$

Першими двома членами послідовності є $b_1 = 289$ та $b_2 = 145$. Якщо ми почнемо з $b_1$ і $b_2$ бобів у двох сусідніх мисках, то нам потрібно було б 3419100 кроків, щоб завершити гру.

Тепер уявимо, що в нас є 1500 сусідніх мисок, які містять $b_1, b_2, \ldots, b_{1500}$ бобів відповідно, а всі інші миски — пусті. Визначте, скільки кроків знадобиться, щоб закінчити гру.

# --hints--

`spillingTheBeans()` має повернути `150320021261690850`.

```js
assert.strictEqual(spillingTheBeans(), 150320021261690850);
```

# --seed--

## --seed-contents--

```js
function spillingTheBeans() {

  return true;
}

spillingTheBeans();
```

# --solutions--

```js
// solution required
```

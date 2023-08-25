# Algoritme


## Тема 1.1 | Швидкість Відпрацювання Алгориму

Швидкість відпрацювання алгоритму визначається його часовою складністю, яка в аналізі алгоритмів виражається у величині О-велике (O-notation). Ця нотація допомагає оцінити, як змінюється час виконання алгоритму зі зростанням розміру вхідних даних (n). Основна ідея полягає в тому, щоб визначити, як змінюється кількість операцій алгоритму при збільшенні об'єму вхідних даних, і виразити цю залежність у вигляді математичного виразу.

1. O(1) - константний час:
Алгоритм має постійний час виконання незалежно від розміру вхідних даних.

Приклад: Доступ до елементу за індексом в масиві.

2. O(log(n)) - логарифмічний час:
Час виконання зростає логарифмічно зі збільшенням розміру вхідних даних.

Приклад: Пошук елементу в відсортованому масиві за допомогою бінарного пошуку.

3. O(n) - лінійний час:
Час виконання зростає лінійно зі збільшенням розміру вхідних даних.

Приклад: Пошук максимального елементу в несортованому масиві.

4. O(n log(n)) - лінійнийіт логарифмічний час:
Час виконання зростає немного швидше, ніж лінійно, але повільніше, ніж лінійно-квазіадитивний час.

Приклад: Швидке сортування (QuickSort).

5. O(n^2) - квадратичний час:
Час виконання зростає квадратично зі збільшенням розміру вхідних даних.

Приклад: Сортування бульбашкою (Bubble Sort).

6. O(2^n) - експоненційний час:
Час виконання зростає експоненційно зі збільшенням розміру вхідних даних.

Приклад: Розв'язання задачі комівояжера за допомогою повного перебору.

> :pushpin:
> Нижче знаходяться вправи для закріплення матеріалу
> 
<details>
<summary> Вправи для закріплення </summary>

### Наведіть час виконання «О-велике» для кожного з наступних сценаріїв.

- [ ] Відоме прізвище, потрібно знайти номер у телефонній книзі.
- [ ] Відомий номер, потрібно знайти прізвище телефонної книги. (Підказка: вам доведеться провести пошук по всій книзі!)
- [ ] Потрібно прочитати телефони всіх людей телефонної книги.
- [ ] Потрібно прочитати телефони всіх людей, прізвища яких починаються з літери "А". (Питання з каверзою!)

</details>

> :books:
> Нижче знаходяться додаткові пам'ятки

<details>
<summary> Додатково </summary>

### 

- [x] Бінарний пошук працює набагато швидше, ніж простий.
- [x] Час виконання O(log п) швидше О(п), а зі збільшенням розміру списку, в якому шукається значення, воно стає набагато швидшим.
- [x] Швидкість алгоритмів не вимірюється за секунди.
- [x] Час виконання алгоритму описується зростанням кількості операцій.
- [x] Час виконання алгоритмів виражається як «О-велике.

</details>

## Тема 1.2 | Типи Алгоритмів
### Сортування:
Алгоритми сортування використовуються для організації елементів у певному порядку. Розрізняють такі типи сортування:

Лінійні: Основна характеристика полягає в тому, що кількість порівнянь та перестановок пропорційна кількості елементів.
Приклади: Бульбашкове сортування, Вставне сортування.
Нелінійні: Кількість порівнянь та перестановок може змінюватися в залежності від вхідних даних.
Приклади: Швидке сортування (QuickSort), Злиття (Merge Sort).

### Пошук:
Алгоритми пошуку використовуються для знаходження конкретного елементу у великій колекції даних.

Лінійний пошук: Проходження через елементи послідовно з порівнянням.
Бінарний пошук: Використовується тільки для відсортованих даних, шукає елемент шляхом ділення простору пошуку на піві.
Графові:
Графові алгоритми використовуються для роботи з графами (наборами вузлів, пов'язаних ребрами).

Алгоритми пошуку в ширину (BFS) та в глибину (DFS): Використовуються для обходу графів та знаходження шляхів між вузлами.
Алгоритм Дейкстри: Використовується для знаходження найкоротших шляхів у вагованих графах.
Алгоритм Прима та Крускала: Використовуються для знаходження мінімального остовного дерева.
### Жадібні алгоритми:
Жадібні алгоритми роблять локально оптимальні вибори на кожному кроці в надії, що це призведе до глобально оптимального результату.
Приклади: Алгоритм Дейкстри, Жадібний алгоритм для задачі охоплення множини.

### Динамічне програмування:
Алгоритми динамічного програмування розбивають великі проблеми на менші підзадачі і зберігають результати підзадач для ефективного використання.
Приклади: Задача рюкзака, Задача про найкоротший шлях, Редакційна відстань.

### Математичні алгоритми:
Ці алгоритми використовують математичні методи для розв'язання конкретних завдань.

Алгоритм Евкліда: Використовується для знаходження найбільшого спільного дільника.
Алгоритм RSA: Використовується для шифрування та дешифрування повідомлень.


## Тема 2.1 | Масиви і Звя'зні списки
Масив - це структура даних у програмуванні, яка дозволяє зберігати та упорядковувати набір однотипних елементів під однією змінною. Основна ідея полягає у тому, щоб мати зручний спосіб доступу до кожного елемента масиву за допомогою індексу, який вказує на його позицію в масиві. У більшості мов програмування індекси масивів починаються з нуля. Це означає, що перший елемент масиву буде мати індекс 0, другий - індекс 1 і так далі. Масиви можуть бути одновимірними (містять одну лінію елементів) та багатовимірними (матриці, куби та інші форми).

Пов'язаний список - це структура даних у програмуванні, яка дозволяє зберігати та упорядковувати набір елементів, кожен з яких містить саму інформацію та вказівку на наступний елемент у списку. Кожен елемент такого списку називається "вузол". Основна відмінність між масивом та пов'язаним списком полягає у способі зберігання та доступу до даних. У масивах ми маємо прямий доступ до елементів за допомогою їх індексів, а в пов'язаних списках доступ до елементів здійснюється за допомогою послідовної навігації від одного вузла до наступного.

Кожен вузол пов'язаного списку містить два основних поля:

1. Дані: Інформація, яку ми зберігаємо у вузлі.
2. Вказівник на наступний вузол: Це посилання на наступний вузол у списку.

Така структура дозволяє створювати зв'язок між вузлами, утворюючи послідовність елементів. Останній вузол вказує на null або спеціальне значення, що позначає кінець списку.

Дії над ціми структурами даних




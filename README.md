# GitBasics
<h2> <b> 1.	Фінальні приготування </b> </h2>

1.1.	Встановлюємо ім'я та адресу електронної пошти для підпису зроблених вами змін.
<p align="left"> <img src="Screenshots/1.1.png" alt="Зображення 1.1"/> </p>
1.2.	Налаштовуємо <b>main</b> як назву гілки за замовчуванням.
<p align="left"> <img src="Screenshots/1.2.png" alt="Зображення 1.2"/> </p>
1.3.	Щоб автоматично керувати закінченнями рядків і попереджати про можливі проблеми, але не блокувати виконання операцій, потрібно виконати команди (для користувачів Windows): <b>git config --global core.autocrlf true</b> та <b>git config --global core.safecrlf warn</b>.
<p align="left"> <img src="Screenshots/1.3.png" alt="Зображення 1.3"/> </p>

<h2> <b> 2.	Створення проекту </b> </h2>

2.1.	Створюємо сторінку «Hello, World»: <br></br>
ㅤ•  Створюємо папку <b>work</b>, потім переходимо до неї та створюємо файл <b>hello.html</b>. <br></br>
Скріншот команди:
<p align="left"> <img src="Screenshots/2.1.а.png" alt="Зображення 2.1.a"/> </p>
Скріншот результату створення папки:
<p align="left"> <img src="Screenshots/2.1.б.png" alt="Зображення 2.1.б"/> </p>
Скріншот результату створення файлу:
<p align="left"> <img src="Screenshots/2.1.в.png" alt="Зображення 2.1.в"/> </p>
ㅤ•  В створеному файлі додаємо зміст, зображений на скріншоті:
<p align="left"> <img src="Screenshots/2.1.г.png" alt="Зображення 2.1.г"/> </p>
2.2. Створюємо репозиторій за допомогою команди <b>git init</b>. 
<p align="left"> <img src="Screenshots/2.2.png" alt="Зображення 2.2"/> </p>
2.3.	Додаємо сторінку у репозиторій.
<p align="left"> <img src="Screenshots/2.3.png" alt="Зображення 2.3"/> </p>

<h2> <b> 3.	Перевірка стану </b> </h2>

3.1.	Перевіряємо поточний стан репозиторія, використовуючи команду <b>git status</b>.
<p align="left"> <img src="Screenshots/3.png" alt="Зображення 3"/> </p>

<h2> <b> 4. Внесення змін </b> </h2>

4.1. Змінюємо вміст файлу <b>hello.html</b>, додаючи до вітання <b>HTML</b>-тег.
<p align="left"> <img src="Screenshots/4.1.png" alt="Зображення 4.1"/> </p>
4.2. Перевіряємо стан робочої директорії.
<p align="left"> <img src="Screenshots/4.2.png" alt="Зображення 4.2"/> </p>

<h2> <b> 5.	 Індексація змін </b> </h2>

5.1.	Проіндексуємо та перевіримо стан.
<p align="left"> <img src="Screenshots/5.png" alt="Зображення 5"/> </p>

<h2> <b> 7.	 Індексація та коміт </b> </h2>

7.1.	Закомітимо зміни: <br></br>
ㅤ•  Зробимо коміт, використавши команду <b>git commit</b>, після чого відкриється редактор з текстом, вписуємо в першому рядку коментар <b>Added h1 tag</b>, зберігаємо зміни.
<p align="left"> <img src="Screenshots/7.1.а.png" alt="Зображення 7.1.а"/> </p>
ㅤ•  Виходимо з редактору. Після цього <b>Git</b> виведе повідомлення про успішний коміт.
<p align="left"> <img src="Screenshots/7.1.б.png" alt="Зображення 7.1.б"/> </p>
7.2.	Перевіряємо стан. 
<p align="left"> <img src="Screenshots/7.2.png" alt="Зображення 7.2"/> </p>

<h2> <b> 8. Зміни, а не файли </b> </h2>

8.1. Виконуємо першу зміну: додаємо стандартні теги сторінок <b>html</b> й <b>body</b> до файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/8.1.png" alt="Зображення 8.1"/> </p>
8.2. Додаємо ці зміни, використовуючи команду <b>git add file</b>.
<p align="left"> <img src="Screenshots/8.2.png" alt="Зображення 8.2"/> </p>
8.3. Виконуємо другу зміну: додаємо заголовок <b>HTML</b> (секцію <b>head</b>) до файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/8.3.png" alt="Зображення 8.3"/> </p>
8.4. Перевіряємо поточний статус.
<p align="left"> <img src="Screenshots/8.4.png" alt="Зображення 8.4"/> </p>
8.5. Робимо коміт, а потім ще раз перевіряємо стан.
<p align="left"> <img src="Screenshots/8.5.png" alt="Зображення 8.5"/> </p>
8.6. Додаємо другу зміну та перевіряємо статус.
<p align="left"> <img src="Screenshots/8.6.png" alt="Зображення 8.6"/> </p>
8.7. Робимо коміт другої зміни.
<p align="left"> <img src="Screenshots/8.7.png" alt="Зображення 8.7"/> </p>

<h2> <b> 9.	Історія проекту </b> </h2>

9.1.	Перегляд історії та однорядковий формат перегляду: <br></br>
ㅤ•  Для отримання списку зроблених змін використовуємо команду <b>git log</b>.
<p align="left"> <img src="Screenshots/9.1.а.png" alt="Зображення 9.1.а"/> </p>
ㅤ•  Якщо додати до цієї команди <b>--pretty=oneline</b>, то можемо переглядати історію в один ряд. 
<p align="left"> <img src="Screenshots/9.1.б.png" alt="Зображення 9.1.б"/> </p>
9.2.	Існує величезна кількість варіантів перегляду історії. Наприклад, перегляд 2 останніх зроблених змін, усіх змін зроблені до чи після 5 хвилин тому, усіх змін зробленим певним автором або навіть вивести усю історію.
<p align="left"> <img src="Screenshots/9.2.png" alt="Зображення 9.2"/> </p>
9.3. Для перегляду змін, зроблених за останній тиждень, виконуємо команду, зображену в наведеному скріншоті, де <b>%h</b> — скорочений хеш коміту, <b>%ad</b> — дата коміту, <b>%s</b> — коментар, <b>%d</b> — доповнення коміту («голови» гілок та теги), <b>%an</b> — ім'я автора.
<p align="left"> <img src="Screenshots/9.3.png" alt="Зображення 9.3"/> </p>
9.4.	Кінцевий формат історії: <br></br>
ㅤ•  Для зручного перегляду історії комітів, виконуємо команду, зображену в наведеному скріншоті, де <b>--pretty="..."</b> — формат виходу, <b>%h</b> — скорочений хеш коміту, <b>%ad</b> — дата коміту, <b>|</b> — візуальний роздільник, <b>%s</b> — коментар, <b>%d</b> — доповнення коміту («голови» гілок та теги), <b>%an</b> — ім'я автора, <b>--date=short</b> — короткий формат дати.
<p align="left"> <img src="Screenshots/9.4.а.png" alt="Зображення 9.4.а"/> </p>
ㅤ•  Налаштуємо кінцевий формат історії за замовчуванням.
<p align="left"> <img src="Screenshots/9.4.б.png" alt="Зображення 9.4.б"/> </p>

<h2> <b> 10.	Отримання старих версій </b> </h2>

10.1.	Отримання хешів попередніх комітів: <br></br>
ㅤ•  Продивимося історію змін.
<p align="left"> <img src="Screenshots/10.1.а.png" alt="Зображення 10.1.а"/> </p>
ㅤ•  Повертаємо робочу директорію до першого коміту, використавши команду <b>checkout</b> та перевіряємо вміст файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/10.1.б.png" alt="Зображення 10.1.б"/> </p>
10.2. Повертаємося до останньої версії в гілці <b>main</b> за допомогою команди <b>switch</b>.
<p align="left"> <img src="Screenshots/10.2.png" alt="Зображення 10.2"/> </p>

<h2> <b> 11.	Створення тегів версій </b> </h2>

11.1.	Створюємо тег першої версії.
<p align="left"> <img src="Screenshots/11.1.png" alt="Зображення 11.1"/> </p>
11.2.	Теги для попередніх версій: <br></br>
ㅤ•  Перемикаємося на коміт, попередній до <b>v1</b>.
<p align="left"> <img src="Screenshots/11.2.а.png" alt="Зображення 11.2.а"/> </p>
ㅤ•  Для цієї версії створюємо тег <b>v1-beta</b>.
<p align="left"> <img src="Screenshots/11.2.б.png" alt="Зображення 11.2.б"/> </p>
11.3.	Перемикаємося за іменами тегу.
<p align="left"> <img src="Screenshots/11.3.png" alt="Зображення 11.3"/> </p>
11.4. Переглянемо теги за допомогою команди <b>git tag</b>. 
<p align="left"> <img src="Screenshots/11.4.png" alt="Зображення 11.4"/> </p>
11.5. Переглянемо теги у логах.
<p align="left"> <img src="Screenshots/11.5.png" alt="Зображення 11.5"/> </p>

<h2> <b> 12. Скасування локальних змін (до індексації) </b> </h2>

12.1. Переходимо на гілку <b>main</b>.
<p align="left"> <img src="Screenshots/12.1.png" alt="Зображення 12.1"/> </p>
12.2. Змінюємо <b>hello.html</b>, додаючи небажаний коментар.
<p align="left"> <img src="Screenshots/12.2.png" alt="Зображення 12.2"/> </p>
12.3. Перевіряємо стан.
<p align="left"> <img src="Screenshots/12.3.png" alt="Зображення 12.3"/> </p>
12.4. Використовуємо <b>checkout</b> для скасування змін в робочій директорії, перемикаючись в версію файлу <b>hello.html</b> у репозиторії.
<p align="left"> <img src="Screenshots/12.4.png" alt="Зображення 12.4"/> </p>

<h2> <b> 13.	Скасування проіндексованих змін (перед комітом) </b> </h2>

13.1.	Внесення змін у файл і їх індексація: <br></br>
ㅤ•  Вносимо зміни у файл <b>hello.html</b>, додаючи небажаний коментар.
<p align="left"> <img src="Screenshots/13.1.а.png" alt="Зображення 13.1.а"/> </p>
ㅤ•  Проіндексуємо ці зміни.
<p align="left"> <img src="Screenshots/13.1.б.png" alt="Зображення 13.1.б"/> </p>
13.2. Перевіряємо стан.
<p align="left"> <img src="Screenshots/13.2.png" alt="Зображення 13.2"/> </p>
13.3. Скасуємо індексацію змін за допомогою команди <b>reset</b>.
<p align="left"> <img src="Screenshots/13.3.png" alt="Зображення 13.3"/> </p>
13.4. Переходимо на версію коміту.
<p align="left"> <img src="Screenshots/13.4.png" alt="Зображення 13.4"/> </p>

<h2> <b> 14.	Скасування комітів </b> </h2>

14.1.	Зміна файлу та виконання коміту: <br></br>
ㅤ•  Змінимо файл <b>hello.html</b>, додаючи небажаний коментар.
<p align="left"> <img src="Screenshots/14.1.а.png" alt="Зображення 14.1.а"/> </p>
ㅤ•  Виконуємо коміт.
<p align="left"> <img src="Screenshots/14.1.б.png" alt="Зображення 14.1.б"/> </p>
14.2.	Виконуємо коміт з новими змінами, що скасовують попередні.
Скріншот команди:
<p align="left"> <img src="Screenshots/14.2.а.png" alt="Зображення 14.2.а"/> </p>
Скріншот редактору:
<p align="left"> <img src="Screenshots/14.2.б.png" alt="Зображення 14.2.б"/> </p>  
14.3. Перевіряємо лог.
<p align="left"> <img src="Screenshots/14.3.png" alt="Зображення 14.3"/> </p>

<h2> <b> 15.	Видалення комітів з гілки (revert) </b> </h2>

15.1. Для початку позначимо останній коміт тегом.
<p align="left"> <img src="Screenshots/15.1.png" alt="Зображення 15.1"/> </p>
15.2. Використовуючи <b>reset</b>, відкатуємо до коміту, що передує до <b>oops</b>. Параметр <b>--hard</b> вказує, що робоча директорія повинна бути відновлена до того стану, що відповідає <b>HEAD</b>-коміту гілки.
<p align="left"> <img src="Screenshots/15.2.png" alt="Зображення 15.2"/> </p>
15.3. Переглянувши усі коміти, можемо побачити, що помилкові коміти не зникли.
<p align="left"> <img src="Screenshots/15.3.png" alt="Зображення 15.3"/> </p>

<h2> <b> 16.	Видалення тегу oops </b> </h2>

16.1. Видаляємо тег <b>oops</b>.  
<p align="left"> <img src="Screenshots/16.png" alt="Зображення 16"/> </p>  

<h2> <b> 17.	Внесення змін до комітів </b> </h2>

17.1.	Зміна сторінки, а потім виконання коміту: <br></br>
ㅤ•  Додаємо в <b>hello.html</b> коментар автора.
<p align="left"> <img src="Screenshots/17.1.а.png" alt="Зображення 17.1.а"/> </p>
ㅤ•  Виконуємо коміт.
<p align="left"> <img src="Screenshots/17.1.б.png" alt="Зображення 17.1.б"/> </p>
17.2. Додаємо в <b>hello.html</b> e-mail.
<p align="left"> <img src="Screenshots/17.2.png" alt="Зображення 17.2"/> </p>
17.3. Змінюємо попередній коміт.
<p align="left"> <img src="Screenshots/17.3.png" alt="Зображення 17.3"/> </p>
17.4. Переглянемо історію.
<p align="left"> <img src="Screenshots/17.4.png" alt="Зображення 17.4"/> </p>

<h2> <b> 18.	Створення гілки </b> </h2>

18.1.	Створюємо гілку.
<p align="left"> <img src="Screenshots/18.1.png" alt="Зображення 18.1"/> </p>
18.2.	Додавання файлу стилів <b>style.css</b>: <br></br>
ㅤ•  Створюємо файл <b>style.css</b>. <br></br>
Скріншот команди:
<p align="left"> <img src="Screenshots/18.2.а.png" alt="Зображення 18.2.а"/> </p>
Скріншот результату створення файлу:
<p align="left"> <img src="Screenshots/18.2.б.png" alt="Зображення 18.2.б"/> </p> 
ㅤ•  В створеному файлі додаємо колір до <b>HTML</b>-тегу з текстом вітання нашого сайту.
<p align="left"> <img src="Screenshots/18.2.в.png" alt="Зображення 18.2.в"/> </p>
ㅤ•  Виконуємо коміт.
<p align="left"> <img src="Screenshots/18.2.г.png" alt="Зображення 18.2.г"/> </p>
18.3.	Зміна <b>hello.html</b> для того, щоб використовувати <b>style.css</b>: <br></br>
ㅤ•  В файлі <b>hello.html</b> додаємо посилання на <b>style.css</b> для стилізації сторінки.
<p align="left"> <img src="Screenshots/18.3.а.png" alt="Зображення 18.3.а"/> </p>
ㅤ•  Виконуємо коміт.
<p align="left"> <img src="Screenshots/18.3.б.png" alt="Зображення 18.3.б"/> </p>
  
<h2> <b> 19.	Перемикання гілок </b> </h2>

19.1.	Перемикання на гілку <b>main</b>: <br></br>
ㅤ•  Переглянемо історію усіх комітів. Можемо побачити, що тепер у нас є дві гілки.
<p align="left"> <img src="Screenshots/19.1.а.png" alt="Зображення 19.1.а"/> </p>
ㅤ•  Перемикаємося між гілками, використовуючи <b>git switch</b> та переглядаємо вміст файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/19.1.б.png" alt="Зображення 19.1.б"/> </p>
19.2. Повертаємося до гілки <b>style</b> та переглядаємо вміст файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/19.2.png" alt="Зображення 19.2"/> </p>
 	
<h2> <b> 20.	Переміщення файлів </b> </h2>

20.1. Переглянемо історію змін файлу <b>hello.html</b>.
<p align="left"> <img src="Screenshots/20.1.png" alt="Зображення 20.1"/> </p>
20.2. Переглянемо різницю між версіями файлу <b>hello.html</b> за допомогою команди <b>show</b>.
<p align="left"> <img src="Screenshots/20.2.png" alt="Зображення 20.2"/> </p>
20.3.	Перейменування <b>hello.html</b>: <br></br>
ㅤ•  Перейменуємо файл <b>hello.html</b>, використавши команду <b>mv</b>. <br></br>
Скріншот команди:
<p align="left"> <img src="Screenshots/20.3.а.png" alt="Зображення 20.3.а"/> </p>
Скріншот результату:
<p align="left"> <img src="Screenshots/20.3.б.png" alt="Зображення 20.3.б"/> </p>
ㅤ•  Додаємо зміну та перевіримо стан.
<p align="left"> <img src="Screenshots/20.3.в.png" alt="Зображення 20.3.в"/> </p>
20.4.	Безпечне переміщення файлу <b>style.css</b>: <br></br>
ㅤ•  Створюємо папку <b>css</b>, безпечно переміщуємо за допомогою <b>git mv</b>, після чого ще раз перевіряємо стан. <br></br>
Скріншот команди:
<p align="left"> <img src="Screenshots/20.4.a.png" alt="Зображення 20.4.а"/> </p>
Скріншот результату створення папки:
<p align="left"> <img src="Screenshots/20.4.б.png" alt="Зображення 20.4.б"/> </p>
Скріншот результату переміщення файлу в папку <b>css</b>:
<img src="Screenshots/20.4.в.png" alt="Зображення 20.4.в"/> </p>
ㅤ•  Закомітимо наші зміни і перевіримо історію змін у файлі <b>css/styles.css</b> та додаємо <b>--follow</b>, щоб побачити історію файлу до того, як він був переміщений.
<p align="left"> <img src="Screenshots/20.4.г.png" alt="Зображення 20.4.г"/> </p>

<h2> <b> 21.	Зміни в гілці main </b> </h2>

21.1.	Створення файлу <b>README</b>: <br></br>
ㅤ•  Створимо файл <b>README</b>.
<p align="left"> <img src="Screenshots/21.1.а.png" alt="Зображення 21.1.а"/> </p>
ㅤ•  В створеному файлі додаємо короткий опис до проекту.
<p align="left"> <img src="Screenshots/21.1.б.png" alt="Зображення 21.1.б"/> </p>
21.2.	Закомітимо файл <b>README</b> у гілку <b>main</b>.
<p align="left"> <img src="Screenshots/21.2.png" alt="Зображення 21.2"/> </p>

<h2> <b> 22.	Перегляд розбіжних гілок </b> </h2>

22.1. Переглянемо поточні гілки у вигляді дерева, скориставшись <b>git log --all --graph</b>, де <b>--all</b> – побачити усі гілки, <b>--graph</b> додає просте дерево комітів, зображене текстовими лініями. 
<p align="left"> <img src="Screenshots/22.png" alt="Зображення 22"/> </p>

<h2> <b> 23.	Злиття </b> </h2>

23.1.	Повернемося до гілки <b>style</b> і зіллємо <b>main</b> із <b>style</b>, потім переглянемо поточні гілки у вигляді дерева. <br></br>
Скріншот редактору:
<p align="left"> <img src="Screenshots/23.а.png" alt="Зображення 23.а"/> </p>
Скріншот команд:
<p align="left"> <img src="Screenshots/23.б.png" alt="Зображення 23.б"/> </p>

<h2> <b> 24.	Створення конфлікту </b> </h2>

24.1.	Повернення у <b>main</b> і створення конфлікту: <br></br>
ㅤ•  Повертаємося до гілки <b>main</b>.
<p align="left"> <img src="Screenshots/24.1.а.png" alt="Зображення 24.1.а"/> </p>
ㅤ•  В файлі <b>hello.html</b> вносимо зміни, а саме дамо назву сайту та абзац.
<p align="left"> <img src="Screenshots/24.1.б.png" alt="Зображення 24.1.б"/> </p>
ㅤ•  Виконуємо коміт.
<p align="left"> <img src="Screenshots/24.1.в.png" alt="Зображення 24.1.в"/> </p>
24.2. Переглянемо гілки.
<p align="left"> <img src="Screenshots/24.2.png" alt="Зображення 24.2"/> </p>

<h2> <b> 25.	Вирішення конфліктів </b> </h2>

25.1.	Злиття <b>main</b> до гілки <b>style</b>: <br></br>
ㅤ•  Повертаємося до гілки <b>style</b> та зливаємо нещодавні зміни з гілки <b>main</b>.
<p align="left"> <img src="Screenshots/25.1.а.png" alt="Зображення 25.1.а"/> </p>
ㅤ•  Подивимося статус.
<p align="left"> <img src="Screenshots/25.1.б.png" alt="Зображення 25.1.б"/> </p>
ㅤ•  Відкривши <b>index.html</b>, то можна побачити те, що частина, що знаходиться в межах <b><<<<<<< >>>>>>></b> - є конфліктом.
<img src="Screenshots/25.1.в.png" alt="Зображення 25.1.в"/> </p>
25.2.	Скасуємо злиття, скориставшись командою <b>git merge --abort</b>.
<p align="left"> <img src="Screenshots/25.2.png" alt="Зображення 25.2"/> </p>
25.3.	Рішення конфлікту: <br></br>
ㅤ•  Ще раз пробуємо злити нещодавні зміни з гілки <b>main</b>.
<p align="left"> <img src="Screenshots/25.3.а.png" alt="Зображення 25.3.а"/> </p>
ㅤ•  Редагуємо файл до наступного стану, як показано на скріншоті.
<p align="left"> <img src="Screenshots/25.3.б.png" alt="Зображення 25.3.б"/> </p>
25.4. Зробимо коміт з розв'язаним конфліктом та подивимося на поточний стан.
<p align="left"> <img src="Screenshots/25.4.png" alt="Зображення 25.4"/> </p>

<h2> <b> 27.	 Відкочування гілки style </b> </h2>

27.1. Відкатуємо гілку <b>style</b> до останнього коміту перед злиттям, тобто за 2 коміти до <b>HEAD</b> за допомогою команди <b>reset</b>. <br></br>
Скріншот команд:
<p align="left"> <img src="Screenshots/27.1.а.png" alt="Зображення 27.1.а"/> </p>
Скріншот резульату відкату:
<p align="left"> <img src="Screenshots/27.1.б.png" alt="Зображення 27.1.б"/> </p>
27.2. Перевіряємо гілку. 
<p align="left"> <img src="Screenshots/27.2.png" alt="Зображення 27.2"/> </p>

<h2> <b> 28.	Перебазування </b> </h2>

28.1.	Перебазування гілки <b>style</b> на <b>main</b>: <br></br>
ㅤ•  Перенесемо зміни до гілки <b>style</b> за допомогою команди <b>rebase</b>.
<p align="left"> <img src="Screenshots/28.1.а.png" alt="Зображення 28.1.а"/> </p>
ㅤ•  Конфлікт стався в файлі <b>hello.html</b>, а не в <b>index.html</b> через те, що <b>rebase</b> був у процесі застосування змін <b>style</b> поверх гілки <b>main</b>. У той момент в гілці <b>main</b> ще не було перейменовано файл <b>hello.html</b>, тому він все ще має стару назву.
<img src="Screenshots/28.1.б.png" alt="Зображення 28.1.б"/> </p>
28.2.	Розв'язування конфлікту: <br></br>
ㅤ•  Відредагуємо файл, щоб він відповідав скріншоту.
<p align="left"> <img src="Screenshots/28.2.а.png" alt="Зображення 28.2.а"/> </p>
ㅤ•  Додаємо усі зміни до індексу та продовжимо процес перебазування. <br></br>
Скріншот редактору:
<p align="left"> <img src="Screenshots/28.2.б.png" alt="Зображення 28.2.б"/> </p>
Скріншот команд:
<p align="left"> <img src="Screenshots/28.2.в.png" alt="Зображення 28.2.в"/> </p>
ㅤ•  Подивимося на поточний стан та гілки.
<p align="left"> <img src="Screenshots/28.2.г.png" alt="Зображення 28.2.г"/> </p>

<h2> <b> 29.	Злиття в гілку main </b> </h2>

29.1. Зливаємо <b>style</b> в <b>main</b>.
<p align="left"> <img src="Screenshots/29.1.png" alt="Зображення 29.1"/> </p>
29.2. Переглянемо логи.
<p align="left"> <img src="Screenshots/29.2.png" alt="Зображення 29.2"/> </p>

<h2> <b> 30.	Клонування репозиторіїв </b> </h2>

30.1. Перейдемо в директорію <b>repositories</b>, глянемо поточну директорію, де зараз знаходимося, та виведемо його вміст.
<p align="left"> <img src="Screenshots/30.1.png" alt="Зображення 30.1"/> </p>
30.2. Створюємо клон репозиторія <b>work</b> та виведемо вміст директорії. <br></br> 
Скріншот команд:
<p align="left"> <img src="Screenshots/30.2.а.png" alt="Зображення 30.2.а"/> </p> 
Скріншот результату клонування:
<p align="left"> <img src="Screenshots/30.2.б.png" alt="Зображення 30.2.б"/> </p>

<h2> <b> 31.	Перегляд клонованого репозиторія </b> </h2>

31.1. Подивимося на клонований репозиторій.
<p align="left"> <img src="Screenshots/31.1.png" alt="Зображення 31.1"/> </p>
31.2. Переглянемо історію репозиторія.
<p align="left"> <img src="Screenshots/31.2.png" alt="Зображення 31.2"/> </p>

<h2> <b> 32.	Що таке origin? </b> </h2>

32.1.	Що таке <b>origin</b>: <br></br>
ㅤ•  Виведемо список віддалених репозиторіїв, з якими пов'язаний наш репозиторій. На виході отримаємо ім'я за замовчуванням віддаленого репозиторія <b>origin</b>.
<p align="left"> <img src="Screenshots/32.а.png" alt="Зображення 32.а"/> </p>
ㅤ•  Подивімось детальну інформацію про ім'я за замовчуванням.
<p align="left"> <img src="Screenshots/32.б.png" alt="Зображення 32.б"/> </p>

<h2> <b> 33.	Віддалені гілки </b> </h2>

33.1.	Віддалені гілки: <br></br>
ㅤ•  Подивімось на гілки, доступні в нашому клонованому репозиторії за допомогою <b>git branch</b>.
<p align="left"> <img src="Screenshots/33.а.png" alt="Зображення 33.а"/> </p>
ㅤ•  Щоб побачити всі гілки, до команди додаємо <b>-a</b>.
<p align="left"> <img src="Screenshots/33.б.png" alt="Зображення 33.б"/> </p>

<h2> <b> 34.	Зміна оригінального репозиторія </b> </h2>

34.1.	Внесення змін в оригінальний репозиторій <b>work</b>: <br></br>
ㅤ•  У файл <b>README</b> в наступному рядку додаємо <b>(changed in origin)</b>.
<p align="left"> <img src="Screenshots/34.а.png" alt="Зображення 34.а"/> </p>
ㅤ•  Додаємо цю зміну і зробимо коміт.
<p align="left"> <img src="Screenshots/34.б.png" alt="Зображення 34.б"/> </p>

<h2> <b> 35.	Підтягування змін </b> </h2>

35.1.	Підтягування змін: <br></br>
ㅤ•  Переходимо до репозиторію <b>home</b> та підтягуємо нові коміти з віддаленого репозиторія, використавши <b>git fetch</b>.
<p align="left"> <img src="Screenshots/35.а.png" alt="Зображення 35.а"/> </p>
ㅤ•  Перевіряємо файл <b>README</b>.
<p align="left"> <img src="Screenshots/35.б.png" alt="Зображення 35.б"/> </p>

<h2> <b> 36.	Злиття підтягнутих змін </b> </h2>

36.1. Зливаємо підтягнуті зміни в локальну гілку <b>main</b>.
<p align="left"> <img src="Screenshots/36.1.png" alt="Зображення 36.1"/> </p> 
36.2. Ще раз перевіряємо зміст файлу <b>README</b>. 
<p align="left"> <img src="Screenshots/36.2.png" alt="Зображення 36.2"/> </p>

<h2> <b> 37.	Додавання гілки відстеження </b> </h2>

37.1. Додаємо локальну гілку, яка відстежує віддалену гілку.
<p align="left"> <img src="Screenshots/37.png" alt="Зображення 37"/> </p>

<h2> <b> 38.	Чисті репозиторії </b> </h2>

38.1.	Перейдемо в директорію <b>repositories</b>, створюємо чистий репозиторій та виведемо його вміст. <br></br> 
Скріншот команд:
<p align="left"> <img src="Screenshots/38.а.png" alt="Зображення 38.а"/> </p>
Скріншот результату створення чистого репозиторію:
<p align="left"> <img src="Screenshots/38.б.png" alt="Зображення 38.б"/> </p>

<h2> <b> 39.	Додавання віддаленого репозиторія </b> </h2>

39.1. Додаємо репозиторій <b>work.git</b> до нашого оригінального репозиторію.
<p align="left"> <img src="Screenshots/39.png" alt="Зображення 39"/> </p>

<h2> <b> 40.	Відправка змін </b> </h2>

40.1.	Відправка змін: <br></br>
ㅤ•  В файлі <b>README</b> змінюємо другий рядок на <b>(changed in the origin and pushed to shared)</b>.
<p align="left"> <img src="Screenshots/40.а.png" alt="Зображення 40.а"/> </p>
ㅤ•  Робимо коміт змін.
<p align="left"> <img src="Screenshots/40.б.png" alt="Зображення 40.б"/> </p>
ㅤ•  Надсилаємо зміни до спільного репозиторія.
<p align="left"> <img src="Screenshots/40.в.png" alt="Зображення 40.в"/> </p>

<h2> <b> 41.	Підтягування спільних змін </b> </h2>

41.1.	Підтягування спільних змін: <br></br>
ㅤ•  Перемикаємось в репозиторій <b>home</b>.
<p align="left"> <img src="Screenshots/41.а.png" alt="Зображення 41.а"/> </p>
ㅤ•  Підтягуємо зміни, щойно відправлені в спільний репозиторій.
<p align="left"> <img src="Screenshots/41.б.png" alt="Зображення 41.б"/> </p>

<h2> <b> 42.	Розміщення ваших Git репозиторіїв </b> </h2>

42.1.	Запуск <b>Git</b>-сервера: <br></br>
ㅤ•  За допомогою <b>git daemon</b> запускаємо <b>Git</b>-сервер.
<p align="left"> <img src="Screenshots/42.а.png" alt="Зображення 42.а"/> </p>
ㅤ•  Тепер в окремому вікні термінала переходимо до директорії <b>repositories</b>, клонуємо репозиторій <b>work.git</b> у нову папку <b>network_work</b> через локальний <b>Git</b>-сервер.
<p align="left"> <img src="Screenshots/42.б.png" alt="Зображення 42.б"/> </p>

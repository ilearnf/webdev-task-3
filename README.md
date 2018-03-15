# Задача «Павел слишком занят»

Перед выполнением задания внимательно прочитайте:

- [О всех этапах проверки задания](https://github.com/urfu-2017/guides/blob/master/workflow/overall.md)
- [Как отправить пулл](https://github.com/urfu-2017/guides/blob/master/workflow/pull.md)
- [Как пройти тесты](https://github.com/urfu-2017/guides/blob/master/workflow/test.md)
- Правила оформления [javascript](https://github.com/urfu-2017/guides/blob/master/codestyle/js.md), [HTML](https://github.com/urfu-2017/guides/blob/master/codestyle/html.md) и [CSS](https://github.com/urfu-2017/guides/blob/master/codestyle/css.md) кода

## Основное задание
Билли безумно рад, что ему помогли сделать `REST-API` сервиса для путешественников.
Однако, ему снова требуется помощь. Реализовывать веб-интерфейс для этого сервиса должен был Паша,
друг Билли, но он, к сожалению, не отвечает в Telegram'е. И Билли, как обычно, попросил помощи у вас.

Предполагается, что реализованный интерфейс будет взаимодействовать с `REST-API`,
написанным вами в предыдущей задаче. Чтобы было проще работать с ним,
выложите его во внешний мир при помощи [now](https://zeit.co/now).

### Требования
Общие:
- В качестве веб-сервера использовать `Express`
- Использовать чистый `DOM-API`, клиентские фреймворки запрещены
- Страница полностью интерактивна, при взаимодействии пользователя с сервисом она не перезагружается

Функциональные:<br/>
  <img src="https://user-images.githubusercontent.com/7279995/37426983-c4c71a18-27e9-11e8-98f7-ad640fde523f.JPG" width="500" alt="main"/>
- Поисковое поле:
	- Вся фильтрация должна происходить в браузере, без взаимодействия с сервером
	- На странице отображаются только те места, которые подходят под введенный пользователем запрос
	- Фильтрация должна учитывать состояние контролла "все"/"посетить"/"посещённые"
- Форма создания места
- Список мест:
	- Имеется кнопка "очистить список"
	- Имеется контрол "все"/"посетить"/"посещённые". В зависимости от состояния показываются
	  только соответствующие места
- Элемент списка:
	- Состоит из названия, контроллов перемещения (можно сделать `drag and drop`) и чекбокса
	- При нажатии на чекбокс непосещённого места, оно помечается как посещённое, и наоборот
	- При наведении на место появляются контроллы для редактирования и удаления
	  <img src="https://user-images.githubusercontent.com/7279995/37427089-11bf637a-27ea-11e8-9dc0-4fea2d8918f2.png" width="300" alt="hover"/>
	- При нажатии на "редактирование" появляется инпут с текущим названием и контролы для сохранения и отмены изменений<br/>
      <img src="https://user-images.githubusercontent.com/7279995/37426799-608d47ac-27e9-11e8-8b75-88568c1eb930.png" width="300" alt="edit"/>

![pasha](https://user-images.githubusercontent.com/7279995/37428021-d483163e-27ec-11e8-8911-ab0aae78b4ae.jpg)

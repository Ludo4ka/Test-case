# my Test-case

### TEST_CASE1.  
#### Редактирование номера телефона пользователя.  
Условия:  
-Пользователь зарегистрирован на сайте https://www.klm.com  
-Пользователь сайта авторизован  

Ожидаемый результат:  
Номер телефона изменен и отображается в  разделе "Мой профиль" -> "Панель управления"  

1.  Шаг: Зайти на главную страницу сайта, в правом верхнем углу кликнуть на имя пользователя.  
Ожидаемая реакция:Раскрылось выпадающее меню профиля.  
2.  Шаг: Выбрать пункт меню "Мой профиль" и кликнуть на него.  
Ожидаемый результат: Открылась страница редактирования профиля.  
3.  Шаг: Слева в вертикальном меню выбрать "Персональные данные", кликнуть.  
Ожидаемый результат: Открылась страница редактирования персональных данных.  
4.  Шаг: Прокрутить экран вниз до раздела "Контактные данные". Найти строку "Телефон" и нажать кнопку "Изменить".  
Ожидаемый результат: Открылась страница редактирования телефонного номера.  
5.  Шаг: Удалить старный номер телефона, вбить новый номер телефона.  
Ожидаемый результат: В поле "Номер мобильного телефона" отображается введеный номер.  
6. Шаг: Нажать кнопку "Сохранить".  
Ожидаемый результат: Появилось всплывающее окно "Обновление выполнено успешно!"


### TEST_CASE2.  
#### Переход с иконки Fasebook в аккаунт KLM на facebook.com  
Условия:   
-Зайти на главную страницу сайта https://www.klm.com  
-Описание теста: Проверить соответсвует ли иконка тому сайту, куда переходим  
 
 	
1.  Шаг: Прокрутить экран вниз до футера сайта.  
Ожидаемый результат: Отоброжаются иконки социальных сетей.  
2.  Шаг: Кликнуть на иконку facebook.  
Ожидаемый результат: Переход по ссылке https://www.facebook.com/KLM  

### Negative test_cases.  
#### 1.Поменять местами логин и пароль при авторизации  
Условия:   
Есть регистрация аккаунта на сайте klm.com  
1.  Шаг: Зайти на главную ст. сайта. В правом верхнем углу нажать "Вход в систему"  
Ожидаемый результат: Открывается форма авторизации пользователя (запрос логина и пароля)  
2. Шаг: В поле "Логин" ввести корректный Пароль, а в поле "Пароль" ввести корр. логин  
Ожидаемый результат: Появляются подсказки: "Укажите действительный адрес электронной почты", "Введите правильный пароль". Кнопка «Войти в систему» не активна. Авторизация не производится  

#### 2.Ввести Логин с пробелом при авторизации.  
Условия: Есть зарегистрированный аккаунт на klm.com, открылась форма авторизации  
1.  Шаг: Ввести в поле "Логин" правильный логин, начиная с пробела.  
Ожидаемый результат: В поле "Логин" отражается введеный логин.  
2.  Шаг: Ввести в поле "Пароль" правильный пароль.   
Ожидаемый результат: Появлятся подсказка "Укажите действительный адрес электронной почты". Кнопка «Войти в систему» неактивна. Авторизация не производится.

#### 3.Ввод цифр в поле "Имя" (форма регистрации).  
Условия: Сайт klm.com отображает 2-ю стр. форму регистрации "Здравствуйте! Как Вас зовут?"  
1.  Шаг: В поле "Имя" ввести цифры.  
Ожидаемый результат: Появляется сообщерие: "Пожалуйста, используйте только буквы." Кнопка "Продолжить" неактивна.  

#### 4.Ограничение на длину пароля.  
Условия: Сайт klm.com отображает 6-ю стр. формы регистрации "Создайте пароль"   
1. Шаг: В поле "Создайте пароль" ввести  13  символов.  Нажать "Продолжить".  
Ожидаемый результат: Появляется справочное сообщение о  количестве символов в пароле. Кнопка «Продолжить» неактивна.  

#### 5.Аторизация при нажатии кнопки "Назад" в браузере.  
Условия: На сайте klm.com есть зарегистрированный аккаунт.  
1.  Шаг: Зайти на главную ст. сайта. В правом верхнем углу нажать "Вход в систему".   
Ожидаемый результат: Открывается форма авторизации пользователя (запрос логина и пароля).  
2.  Шаг: Ввести корректный логин и пароль. Нажать на кнопку “Назад” в браузере.  
Ожидаемый результат: Снова увидеть форму для авторизации пользователя (запрос логина и пароля).  

#### 6. Прерывание сеанса при отключении интернета.  
Условия: Есть зарегистрированный аккаунт на сайте klm.com  
1.  Шаг: Войти в аккаунт.  
Ожидаемый результат: В правом верхнем углу видим имя профиля.  
2.  Шаг: Отключить интернет  
Ожидаемый результат: Видим "Страница недоступна".  
3.  Шаг: Подключить интернет.  
Ожидаемый результат: Видим сигнал подключения к интернету.  
4.  Шаг: Зашли на сайт klm.com  
Ожидаемый результат: Пользователь не авторизован. В правом верхнем углу есть кнопка "Войти в систему".  

#### 7. Аутентификация через URL-адрес.  
Условия: Пользователь открыл сайт в  браузере и залогинился.  
1.  Шаг: Открыть любую страницу/форму, скопировать URL-адрес.  
Ожидаемый результат: URL-адрес в буфере обмена.  
2.  Шаг: Открыть ДРУГОЙ браузер и вставить туда скопированный URL-адрес.   
Ожидаемый результат: В адресной строке отражается вставленный URL.  
3.  Шаг: Нажать Enter.  
Ожидаемый результат: Открывается форма авторизации пользователя (запрос логина и пароля).  

#### 8. Отправка формы регистрации при двойном клике на кнопку "Продолжить".  
Условия: Пользователь на сайте klm.com открыл форму регистрации и дошел до  7 стр. формы регистрации о принятии правил и условий Flying Blue.   
1.  Шаг: На стр.7 формы регистрации принять "Правила и условий Flying Blue".   
Ожидаемые условия: Видим синию галочку в чекбоксе.  
2.  Шаг: Дважды быстро кликнуть на "Продолжить".  
Ожидаемые условия:  Система регистрирует покупателя (появляется сообщение с номером карты -10 цифр. В базе данных создается ОДНА запись о новом пользователе.  



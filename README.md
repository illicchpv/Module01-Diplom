# Module01-Diplom

## навыки 

### история (для себя)

вопросы

1 - зачем в архиве "макет для дипломной работы.zip"  фонты? Montserrat-Bold.ttf Montserrat-Regular.ttf 

2 - "Диплом Модуль 1 Объяснение.pdf" на стр. UI Kit 
https://c2n.me/4hT79kL
картинки отличаются на 1 пиксель. это реально надо воспроизвести?

3 - не нашел ссылки на Codepen. Подскажите. 
/Верстку галочки (соглашение) я показала в Codepen - это частая ситуация,
когда на сайтах нужно будет реализовывать такие элементы, поэтому
сохраните себе ссылку на Codepen на будущее, пригодится/
    Андрей> https://codepen.io/anna_blok/pen/ZEXaovV

5 - непонятно назначение папок 
files\@1x 
files\@2x 
особенно по поводу банера

https://c2n.me/4hT9cNm

там справа вертикальная полоса которой нет фигме. её надо реализовывать?
    Андрей> @2x  это для ретина экрана
    Андрей> https://developer.mozilla.org/en-US/docs/Web/CSS/@media/-webkit-device-pixel-ratio

///// проблемы
  -переделать hover на расписании так как в \O компании\ 
      // не работает - transition: all var(--trt);
      не получается

  -что делать с ретина экранами?

//// исправлено
  переделать hover на \Ближайшие события\ // кнопки оказываются 
    под появляющимся слоем и не нажимаются
      кнопки перенести на появляющийся слой?

----------------------------------------------------
//исправлено
+ градиент При наведении, перекрывает текст
.event-time {
...
    position: relative;
    z-index: 1;
}
.event-name {
...
    position: relative;
    z-index: 1;
}

//исправлено как смог
+- нога Не совпадает с желтым фоном
.ybackground {
...
  box-sizing: border-box;
  border-bottom: 40px solid white;
}

//непонятно
+ в footer у ссылки не те стили
???	не понял совпадает с макетом. 
	https://c2n.me/4hYQVPT

//исправлено
+ в footer ссылку на электронную почту 


//----------------------------------------------------------
- банер
	https://lapdev.ru/


+ Кнопку можно скрывать на этом разрешении
	880

+ К мобильной версии, здесь расстояние меньше, (про первую строку событий)


+ Можно убирать изображение, к мобильной версии, оно плохо смотрится 
	и его нет в макете на мобилке


+   Можешь на этом разрешении , эти блоки в одну колонку сделать , 
   можно сделать шрифт побольше, а к мобильной версии подогнать под макет размер шрифта
	 460px - 1 col
	.about-infos-block


+ в footer у ссылки не те стили


+ сделай не через тег <a> , а через button , объясню в чем


+ В макете есть отступ снизу, добавь его
	На десктопе он есть, потом куда-то пропадает

	.footer-madeby {
		...
	    margin-bottom: 56px;  // 40
	}


+ ошибка при клике
	прокрутку до расписания тренировок

+ И осталось градиент вернуть
	.event-item-gradient{

//-----------------------------------------------
  + 1. постарайся заполнить пустоту справа .
    @media 545
    .banner-content-block h1 {
        text-align: center;
    .banner-content-block h3 {
        margin-left: 5vw;
    .banner-subblock-text p {
        margin-left: calc(3vw + 35px);
        max-width: 100%;
        text-align: right;

 + 2. между рукой и кнопкой, сделай расстояние, на мобилке ты его сделал, добавь сюда.

 + Немного уменьши заголовок, сильно близко он к изображению
	@media (max-width: 1300px)
		.banner-content-block h1 {
    		font-size: 45px;

 + Еще валидатор немного ругается, в остальном все отлично
//-----------------------------------------------
  - вернуть в зад результаты:
    + 1. постарайся заполнить пустоту справа .
    изменяю фонт h1 в зависимости от ширины

//--------------------------
 + Изображение не совпадает a желтым фоном
    убрал вылезший снизу фон
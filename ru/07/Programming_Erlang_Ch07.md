# Глава 7. Параллельность

<dl>
<dt>Мы понимаем параллельность мира.</dt>
<dd>
Глубокое понимание параллелизма заложено в нашем мозге. Мы реагируем на внешние раздражители очень быстро при помощи отдела нашего мозга, называемого *миндалевидное тело*. Без такого реагирования мы бы довольно скоро погибли. Наше сознание, по сравнению с подобными реакциями, гораздо медленнее. За то время, пока сама мысль "нажми на тормоз" сформируется, это действие будет нами уже выполнено.

Когда мы ведем автомобиль в насыщенном транспортном потоке, мы непроизвольно отслеживаем местоположение и скорость десятков, если не сотен автомобилей. Все это происходит без участия сознания. Если бы мы не умели это делать, мы бы, вероятно, погибли бы на дороге.

</dd>

<dt>Наш мир параллелен.</dt>
<dd>
Если мы хотим писать программы, которые ведут себя подобно другим объектам реального мира, то эти программы должны быть соответствующим образом структурированы.

Писать такие программы надо на параллельном языке программирования.

К сожалению, пока приложения для решения реальных задач пишутся на последовательных языках программирования. А это ведь является излишним усложнением.

Используйте язык, который был специально разработан для написания параллельных приложений и разработка параллельных систем станет намного проще и приятнее!  
</dd>  

<dt>Программы на Эрланге моделируют наш процесс мышления и взаимодействия.</dt>
<dd>
У нас с вами нет общей разделяемой памяти. У меня есть своя память, а у вас — своя. Каждый из нас имеет мозг, по одному на брата. Они не могут быть объединены. Чтобы изменить вашу память, я должен послать вам сообщение: что-то сказать или, хотя бы, помахать рукой.

Вы слушаете, вы смотрите и ваша память изменяется. Но, тем не менее, не задав вам соответствующего вопроса или не видя вашей реакции, я не могу быть уверенным, что вы получили мое сообщение.

Чтобы убедиться в том что другой процесс получил ваше сообщение и изменил свою память, вы должны спросить его об этом (послав ему сообщение). Именно так мы сами и взаимодействуем.

***Сью:*** *Привет, Билл, мой номер телефона — 45 67 89 12.*

***Сью:*** *Ты меня понял?*

***Билл:*** *Конечно, твой номер телефона — 45 67 89 12.*

Подобные стереотипы поведения взаимодействия очень хорошо нам известны. От самого рождения мы учимся, как взаимодействовать с окружающим миром наблюдая за ним. Мы посылаем разного рода сообщения и наблюдаем за ответной реакцией.
</dd>


<dt>Люди функционируют, как независимые сущности, которые общаются с помощью посылки друг другу сообщений.</dt>
<dd>
Именно так работают процессы в Эрланге и именно так работаем и мы сами, а это значит, что нам будет очень просто понять механизмы работы программ написанных на Эрланге.

Программы на Эрланге состоят из десятков, сотен, а иногда и сотен тысяч маленьких процессов. И все они работают независимо друг от друга. Все эти процессы работают независимо. Они общаются между собой путем посылки друг другу сообщений. Каждый процесс имеет свою собственную память. Они ведут себя как большая команда, участники которой переписываются друг с другом.

Это позволяет значительно проще управлять и масштабировать программы на Эрланге. Предположим у нас есть десять людей (процессов) и слишком много работы, которую они должны сделать. Что мы можем сделать в такой ситуации? Позвать на помощь больше людей. А как нам управлять этими группами людей? Это просто — надо просто рассказать им, всем сразу, их инструкции (широковещательное сообщение от одного ко многим).

Процессы в Эрланге не имеют общей памяти, так что нет никакой необходимости в ее блокировке перед ее использованием. Там где есть замки (блокировки) там будут и потерянные ключи к этим замкам. А что происходит, когда вы теряете свой ключ? Вы паникуете и не знаете, что же вам теперь делать. И то же самое происходит в программных системах, теряются ключи и ваши блокировки заклинивает.

Распределенное программное обеспечение с блокировками и ключами к ним, всегда подвержено этому риску и страдает от этого.

А в Эрланге просто нет никаких блокировок и ключей.
</dd>

<dt>Если кто-то умирает, другие люди это заметят.</dt>
<dd>
Если я, находясь в помещении с людьми, вдруг упаду и умру, то кто-то, вероятно, это заметит (ну по крайней мере, я на это надеюсь). Процессы Эрланга в этом подобны людям — они могут внезапно завершиться. Но в отличии от людей, когда они завершаются, они могут громко выкрикнуть на своем последнем вздохе точную причину своей кончины.

Представьте себе комнату полную людей. Неожиданно кто-то из них падает и умирает. И в самый момент своей смерти он произносит: " я умер от сердечного приступа" или "я умер от разрыва слепого отростка желудка". Также поступают и процессы Эрланга. Один процесс, завершаясь, может сообщить: "я умер, потому что меня попросили разделить на ноль". А другой, возможно, сообщит: "я умер, потому что меня спросили каков последний элемент в пустом списке".

А теперь, давайте представим, что в нашей комнате полной людей, есть специально назначенные люди, работа которых заключается в том, чтобы убирать трупы. Давайте представим себе двух людей, Джейн и Джона. Если умирает Джейн, то Джон решает все проблемы, связанные с ее погребением. А если умирает Джон, то все эти проблемы решает Джейн. То есть, получается, что Джейн и Джон как бы связаны между собой незримым соглашением, в котором говорится, что если один из них умирает, то другой разбирается со всеми вопросами связанными со смертью другого.

Именно так работает механизм ошибок в Эрланге. Процессы в нем могут быть связаны вместе. И если один из них прекращается, то другой получает сообщение об ошибке, сообщающее причины его завершения.
</dd>

</dl>

Вот, в основном, и все.

Вот так и работают Эрланг-программы.

Итак, подведём промежуточные итоги:

- Эрланг-программы состоят из множества процессов. Эти процессы посылают друг другу сообщения.

- Эти сообщения могут быть и не приняты адресатом и не поняты им. Если вы хотите точно узнать, что ваше сообщение было получено и понято, вы должны послать соответствующее сообщение этому процессу и ждать его ответа.

- Пары процессов могут быть связаны вместе. Если один из таких связанных процессов прекращается, то другому процессу будет послано сообщение, содержащее в себе указание на причину заверешния первого.

Эту простую модель программирования я называю *параллельно-ориентированное программирование.*


В следующей главе мы начнем писать параллельные программы. Нам потребуется для этого изучить три новых базовых механизма: порождение нового процесса **`spawn`**, **`send`** (с помощью оператора `!` ) и **`receive`**. После чего мы сможем написать несколько простых параллельных программ.

Когда процессы прекращается, другой процесс получает об этом сообщение, если они были с ним связаны. Подробее эта тема рассматривается в Главе 9 *Ошибки в параллельных программах*.

Когда вы будете читать следующие две главы не забывайте о модели множества людей в одной комнате. Люди — это процессы. Люди в комнате имеют каждый свою собственную память — это состояние процесса. Чтобы изменить вашу память, я должен вам что-то сообщить, а вы должны это воспринять и понять. Это и есть посылка и получение сообщений. Дети — это порожденные нами процессы. Сметь — это заверешние процесса.

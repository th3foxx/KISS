+++
title = "Знакомство с ArchLinux"
description = ""
type = ["posts","post"]
tags = [
    "archlinux",
    "kiss",
    "archway",
    "unixway",
]
date = "2022-02-27"
categories = [
    "ArchLinux"
]
series = ["ArchLinux"]
[ author ]
  name = "Th3_Fox"
+++

## Введение

Arch Linux — независимый дистрибутив GNU/Linux для опытных пользователей, оптимизированный для архитектуры x86-64, который стремится предоставить последние «новейшие» версии программ, следуя модели rolling release. По умолчанию пользователю предоставляется минималистичная базовая система, в которую пользователь может добавить то, что ему требуется. Для установки, удаления и обновления пакетов используется пакетный менеджер Pacman.

У Arch Linux есть обширный раздел документации в поддомене ArchWiki, основанный на MediaWiki, который поддерживается разработчиками и сообществом. Документация переведена на десятки языков, однако основным является английский. В документации также можно найти официальное руководство по установке.

Благодаря наличию обширной документации и отсутствию графического установщика, Arch представляет большой академический интерес для тех, кто хочет освоить GNU/Linux.

Arch Linux является независимым дистрибутивом, разработанным с нуля. Создатель дистрибутива Джадд Винет вдохновлялся CRUX, но мнение о том, что Arch основан на CRUX, ошибочно. На Arch основаны такие дистрибутивы, как Antergos, Parabola GNU, ArchBang, Arch Hurd, Chakra, ConnochaetOS, Manjaro и другие.

## Основные особенности Arch

Философия Arch Linux базируется на нескольких основных принципах:

 * **Простота**
 * **Современность**
 * **Прагматизм**
 * Нацеленность на **определенных** пользователей (**user-centric, а не user-friendly**)
 * **Гибкость**

Так разработчики описывают основные особенности и принципы, на которых базируется Arch:

 * Простота. (Заметим, что под простотой подразумевается не простота использования ОС, а простота её внутренней организации: минимализм, лаконичность, следование принципам KISS и Unix-way.)
 
 * Рассчитана не на новичков, а на более опытных пользователей.
 * Джадд Винет основал этот дистрибутив, руководствуясь своим видением идеального дистрибутива, и желая вернуть хоть что-то сообществу свободного программного обеспечения, после того, как столько заимствовал из него.
 * Цель — сделать Arch совершенной основой. Основой, не включающей в себя причудливых утилит и автонастроек, но с утилитами для ручной настройки и некоторыми функциями для пользователей, чтобы они могли продолжить дальнейшую разработку сами.
 * «Вернуть хоть что-то сообществу свободного программного обеспечения» — это свободный дар. Когда вы получаете подарок от кого-либо, это обычно подразумевает, что вам придется что-либо отдать взамен. Так что идеи, предложения, утилиты от пользователей приветствуются.
 * Есть две стороны Arch Linux: сторона разработчика и сторона пользователя. Не надейтесь объединить обе стороны, но создайте между ними взаимную связь, тогда каждый может получить то, что он хочет добавить к своей системе.
 * Не позволяйте утилитам настройки или GUI управлять системой, она должна управляться пользователем. Нет ничего плохого в GUI до тех пор, пока графический интерфейс соответствует этим принципам.
 * Не будьте зависимы от того, что предлагают утилиты. Когда вы пишете или выбираете инструмент, он должен быть написан на читаемом языке программирования (KISS), чтобы позволить пользователям изменить его, если они захотят.
 * Ядро разработки Arch Linux не будет представлено какими-либо «дружественными» GUI/утилитами в ближайшем будущем.
 * Arch будет тем, что вы из него сделаете.
 * Слово «проще» в Arch рассматривается по-другому нежели в других дистрибутивах. Чтобы легко чего-либо достичь, нужно учиться.
 * Надежда на графический интерфейс для настройки/использования системы в конце концов принесёт пользователю только проблемы. В какой-то момент времени пользователь почувствует, что ему нужно знать, что скрывает графический интерфейс.
 * Попытки скрыть сложность системы и сделать её проще за счёт графических утилит и автоматизации рутинных задач обычно приводят к ещё более сложной системе. Вместо этого лучше сделать её более простой и логичной изнутри, разумеется, учитывая ваши задачи, взгляды и предпочтения.
 * Рано или поздно вам потребуется искать информацию в Интернете или в Usenet (если страницы man окажется недостаточно). Уметь искать в сети — это первое, чему должен научиться начинающий пользователь.
 * В то время как пользователи говорят, что такой-то дистрибутив не похож на какой-то другой, Arch позволяет пользователю вносить желаемый вклад до тех пор, пока это не противоречит принципам и философии Arch.
 * Основное свойство возможности сделать свой вклад заключается в том, что вам не нужно разрешение, чтобы его сделать. Никто не может остановить вас при написании того, что вы лично находите полезным, даже если «силы, которые существуют» не считают это благодеянием. Напишите это и поместите в User Contributions форум. Если людям это понравится, вы получите ответ. Даже если предположить, что все вокруг это не оценят, разве вас это будет волновать, если для вас польза очевидна?
 * Не надо требовать от разработчиков утилит и документации. Попытайтесь понять цель и философию Arch — это то, что отличает Arch от других.
 * Единственный бинарный дистрибутив, где собрано все так, как задумали разработчики без каких-либо изменений в исходном коде. По этой причине и появился миф о стабильности Arch Linux.

## Почему стоит попробовать ArchLinux

#### 1. С Arch Linux вы можете создать свой собственный компьютер
Arch Linux является уникальным среди наиболее популярных дистрибутивов Linux. Ubuntu и Fedora, к примеру, похожи на Windows и macOS, тем, что из коробки готовы к работе. В противоположность этому, Arch Linux ставит перед вами задачу создать операционную систему для вашего ПК самостоятельно.

Раньше Arch Linux был очень сложным в установке. Фактически, старый процесс установки Arch Linux можно было использовать для того, чтобы отогнать любопытных потенциальных пользователей. Но теперь это не так, благодаря установщикам с графическим интерфейсом, таким как Anarchy и встроенный в систему с 2021 года скрипт установки.
`Но рекомендуется устанавливать систему своими руками, а не при помощи скриптов, так как это даст более точно настроить систему под себя, это не противоречит принципу ArchWay и даст понимание о том, как она работает.`

Сейчас Arch Linux намного проще установить, чем раньше. Это сводит на нет одну из причин, по которой не стоило устанавливать его.

В конце концов, вы остаетесь с системой, которая делает именно то, что вы хотите. И даже если вы установите дистрибутив на основе Arch, который обеспечивает работу всех компонентов из коробки, вы все равно можете поменять части по своему усмотрению.

#### 2. Вы запускаете только то, что вам нужно
Поскольку Arch позволяет вам выбирать ваши собственные компоненты, это означает, что вы не обременены кучей программного обеспечения, которым вы не намерены пользоваться. Ubuntu не только поставляется с большим количеством предустановленных настольных приложений, но также имеет довольно много фоновых сервисов.

Несмотря на то, что это число мало по сравнению с тем, сколько работает в фоновом режиме в Windows, скорее всего, вы не знаете, что там происходит.

Эти службы не только не работают в Arch Linux по умолчанию, они даже не установлены. Это означает, что вы не тратите ресурсы на дополнительные системные процессы. Вы также экономите пропускную способность интернета, не загружая обновления кода, которые не нужны.

#### 3. Arch Linux хорош технически
Многие дистрибутивы Linux представляют собой бесплатные и простые в использовании альтернативы Windows и macOS. Они хотят привлечь студентов, разработчиков и обычных пользователей. В результате они не выделяют многие “гайки и болты”, которые заставляют систему работать. Они не обязательно скрывают эту информацию, но вы должны знать, где искать и что искать.

Arch не пытается представить себя чем-то другим, кроме набора программ, которые вы можете собрать, чтобы сделать функциональный компьютер. Хотите узнать, какие конкретные пакеты получают обновления или возникают проблемы? Arch размещает эту информацию на главной странице своего сайта. Каждая ссылка, по которой вы нажимаете, только углубляет техническую информацию.

#### 4. Подождите, пока вы не попробуете Pacman в Arch Linux
Pacman – это то, что вы используете для установки пакетов в Arch. Это то, что apt для Ubuntu, а для Fedora dnf. За исключением того, что в отличие от этих дистрибутивов, Arch не изо всех сил пытается навязать графическую альтернативу командной строке.

Одним из преимуществ Pacman является то, что вам не нужно много печатать. Команда для установки определенного пакета:
``` Bash
pacman -S package-name
```
Хотите загрузить последние обновления для всей вашей системы?
``` Bash
pacman -Syu
```
Какой менеджер пакетов вы предпочитаете, зависит от вашего вкуса. Но вы можете обнаружить, что Pacman вам нравится.

#### 5. AUR – пользовательский репозиторий Arch Linux

Arch User Repository представляет собой набор программного обеспечения от членов сообщества, которые Arch еще сам не поддерживает. Вместо того, чтобы загружать исходные файлы приложения самостоятельно и пытаться выяснить, как все работает, AUR выполняет тяжелую работу. Есть хороший шанс, что если вы хотите запустить программу для Linux, которой нет в репозиториях Arch, она находится в AUR.

Использование AUR не сразу интуитивно понятно, но есть способы упростить процесс. Такой инструмент, как Yay, может помочь вам в командной строке, а Octopi (KDE), Pamac (Gnome) предоставляет графический интерфейс, который выполняет фоновую работу за вас.

#### 6. Arch Wiki – лучшее из всех
В настоящее время я использую дистрибутив, созданный на основе Arch Linux, но даже когда у меня его нет, у меня все еще есть много причин, чтобы посетить Arch Wiki. Независимо от того, какой дистрибутив Linux вы используете, Arch Wiki – это клад c информацией.

Поскольку Arch использует те же компоненты, что и большинство других дистрибутивов Linux, руководства содержащиеся на этом сайте, актуальны далеко за пределами экосистемы Arch. Если вы не уверены, какое программное обеспечение установить на свой компьютер, ознакомьтесь с описаниями, представленными здесь. Следуйте инструкциям, прочитайте рекомендации и обратите внимание на ошибки.

Могут быть некоторые различия в том, как ваш дистрибутив и Arch делают разные вещи, но сайт все равно может указывать вам правильное направление.

#### 7. Стабильность и надежность
Метод обновления Arch Linux — плавающий релиз, благодаря чему не нужно беспокоиться о переустановке системы для получения новой версии дистрибутива, как пользователям других дистрибутивов. Поскольку его базовая система всегда обновлена с учетом последних исправлений и новых функций, и вам не нужно беспокоиться о том, когда устанавливать обновление системы и сколько времени оно займет.

Кроме того, каждое обновление совместимо с вашей системой, поэтому не нужно опасаться, что какое то обновление что-то сломает, и это делает Arch Linux одним из самых стабильных и надежных дистрибутивов. (Если обновляться не раз в полгода).

#### 8. Arch имеет меньше корпоративного влияния
Многие люди используют Linux, потому что они не хотят, чтобы компания определяла, что они могут делать на своем компьютере. Независимо от того, какую версию Linux вы используете, коммерческое влияние на работу вашего ПК будет меньше, чем на Windows или macOS. Но, в конце концов, такие дистрибутивы, как Ubuntu, Fedora и openSUSE, по-прежнему связаны с корпоративным спонсором.

Если вы используете дистрибутив, основанный на Ubuntu, на ваш рабочий стол по-прежнему влияют решения, которые принимает Canonical. Подобное влияние гораздо меньше в случае с Fedora и openSUSE. Но если вам нужен еще больший разрыв, вам нужен дистрибутив только для сообщества, такой как Arch.

#### 9. Идеальная учебная база
Arch Linux - это идеальная учебная платформа для всех, кто хочет узнать, как работает Linux, поскольку требует внимания к документации при его использовании.

Конечно, вы можете решить искать быстрые решения и двигаться дальше в своей жизни, но если вы хотите выяснить причину проблем, а также способы их устранения, то Arch Linux и его огромная база знаний хорошая отправная точка.
#### 10. Сообщество Arch Linux
Помимо Arch Wiki, Arch Linux имеет обширное сообщество пользователей, которое добровольно готово предложить помощь всем, кто интересуется изучением Linux, особенно с использованием Arch Linux или любого из его производных дистрибутивов.

Они также посвящены содействию успеху Arch Linux и простоте использования, возьмите Arch User Repository для примера. Хотя, даже если вы застряли в вики, вы в надежных руках.

#### Что можно получить после настройки:
{{< image src="/img/gallery/1.jpg" alt="KDE" position="center" style="border-radius: 8px;" >}}
{{< image src="/img/gallery/2.png" alt="KDE" position="center" style="border-radius: 8px;" >}}
{{< image src="/img/gallery/3.png" alt="KDE" position="center" style="border-radius: 8px;" >}}
{{< image src="/img/gallery/4.png" alt="KDE" position="center" style="border-radius: 8px;" >}}
{{< image src="/img/gallery/5.png" alt="KDE" position="center" style="border-radius: 8px;" >}}


## Так стоит ли мне устанавливать Arch?
Это вам решать. Я всего лишь показал вам некоторые из многих преимуществ Arch. Почему бы вам не взять дистрибутив Arch Linux или более легкую альтернативу и попробовать его сейчас? Если вы обнаружите, что Arch Linux по-прежнему не дает вам достаточного контроля, вы всегда можете попробовать Gentoo:).

#### Использовались следующие источники:
 * [10 причин использовать Arch Linux](https://losst.ru/10-prichin-ispolzovat-arch-linux)
 * [Стоит ли устанавливать Arch Linux? 10 причин](https://komyounity.com/stoit-li-ustanavlivat-arch-linux/)
 * [UnixPorn](https://www.reddit.com/r/unixporn)

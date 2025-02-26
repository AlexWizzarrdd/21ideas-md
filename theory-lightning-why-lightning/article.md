 # Зачем нужна сеть лайтнинг?

Содержание:

1.   Что происходит?
2.   Что такое лайтнинг?
3.   Зачем использовать лайтнинг? Можно ли получить от этого выгоду?
4.   С чего начать?
5.   Как поддерживать проекты, оплачивать заказы и передавать ценность в сети лайтнинг?
6.   Как поддерживать проекты и передавать ценность, не выходя из Telegram?
7.   Как зарабатывать с помощью сети лайтнинг?
8.   Практические примеры.

---

## Что такое лайтнинг?

Сеть лайтнинг _(Lightning Network)_ является децентрализованной системой для мгновенных микроплатежей, которая устраняет риск делегирования ответственного хранения средств доверенным третьим лицам. Биткоин, самая широко используемая и ценная в мире криптовалюта, позволяет любому передать ценность без необходимости в доверенном посреднике или депозитарии. Биткоин поддерживает продвинутую систему скриптов, позволяющую пользователям программировать инструкции по распоряжению собственными средствами. Тем не менее, существует ряд недостатков децентрализованного дизайна Биткоина. С момента совершения сделки на блокчейне Биткоина и до момента, когда эта сделка станет необратимой может пройти час, а часто и намного больше.

Разумеется, микроплатежи, или платежи, не превышающие несколько копеек, на сегодняшний день не выглядят жизнеспособными.

Сеть лайтнинг решает эту проблему. Это одна из первых реализаций многостороннего смарт-контракта (программируемые деньги) с помощью встроенного скрипта протокола Биткоин. Сеть лайтнинг — ведущая технологическая разработка в контексте многопользовательских финансовых расчетов на основе сети Биткоин.

__Мгновенные платежи:__ Биткоин объединяет транзакции в блоки, появляющиеся с интервалом приблизительно в десять минут. Платежи в сети считаются необратимыми по прошествии шести подтверждений (появлении шести блоков поверх блока, содержащего вашу транзакцию) или около часа. В сети лайтнинг платежи не требуют подтверждения и являются мгновенными. Лайтнинг можно использовать в терминалах розничной торговли, между устройствами пользователей или в любой другой ситуации, где необходимы мгновенные платежи.

__Микроплатежи:__ Благодаря появлению микроплатежей могут появиться новые рынки. Лайтнинг позволяет отправить средства вплоть до 0.00000001 биткоина, не вынуждая вас обращаться к кастодиальным сервисам. Минимальная комиссия за транзакцию на блокчейне Биткоина сегодня во много сотен раз выше, а фиксированная плата за транзакцию делает микроплатежи не практичными. Лайтнинг позволяет осуществлять минимальные платежи, номинированные в биткоине, используя фактические биткоин-транзакции.

__Масштабируемость:__ Если сеть Биткоин намерена удовлетворить спрос присоединяюшихся пользователей, она должна поддерживать на порядок больший объем транзакций. В связи с предстоящим ростом количества устройств, подключенных к интернету, требуется платформа для платежей от устройства к устройству и автоматизированные микроплатежи. Транзакции в сети лайтнинг проходят вне блокчейна Биткоина, и также не требуют делегировать доверие и права собственности, что позволяет пользователям проводить практически неограниченное количество операций.

__Как это работает:__ Средства помещаются в двухсторонний [мультисиг](https://www.21ideas.org/theory-security-multisig-1/) биткоин-адрес, также называемый "каналом". Этот канал сохраняется как запись в публичном реестре Биткоина. Для того, чтобы потратить средства из канала, обе стороны должны договориться о последнем балансе. Текущий остаток хранится как последняя сделка, подписанная обеими сторонами, расходующая средства с соответствующего адреса канала. Для осуществления платежа обе стороны подписывают новую транзакцию, инициирующую выход из канала. При этом все старые операции аннулируются.

Для выхода из лайтнинг-канала сеть не требует сотрудничества вашего контрагента. Обе стороны имеют возможность в одностороннем порядке закрыть канал. Так как все участники имеют множественные каналы с многими пользователями сети, отправить платеж любому другому участнику не составляет труда.

Подробнее о сети лайтнинг и ее особенностях вы можете узнать в этом разделе:

[__Lightning Network__. Все, что нужно знать о Lightning Network, втором уровне поверх Биткоина, призванном сделать сеть быстрее, дешевле и приватнее.](https://www.21ideas.org/theory-ln/)

---

## Кому это надо?

В сети лайтнинг на сегодняшний день <a href="https://1ml.com/statistics" rel="noopener noreferrer">насчитывается</a> более 30 тысяч нод и почти 40 тысяч каналов; в сети также заблокировано более тысячи биткоинов (около $50 млн. на момент написания этого материала). Этот протокол уже довольно распространен и продолжает развиваться. С улучшением пользовательского опыта взаимодействия с Биткоином в лайтнинг будет приходить все больше пользователей.

![pic1](https://github.com/LightningTony/bitcoin-guide-pics/blob/main/practical/Zachem_nuzhna_set_lajtning/pictures/pic1.png) 

Быть ранним пользователем любой \*полезной\* сети никогда не будет лишним — вы получаете возможность с меньшими усилиями получить больше ценности (в том или ином виде), чем те, кто присоединится позже вас. Когда разговор заходит о сетях, связанных с финансами, ценность становится еще более ощутимой. На сегодняшний день существует ряд способов получения прибыли (пусть и небольшой на данный момент, но с распространением Биткоина каждый сатоши становится все более ценным), и мы поговорим о некоторых из них далее.

---

## Заработок в сети лайтнинг

Существует множество способов заполучить заветные сатошики: от получения донатов за производство полезных материалов через сервис [Tippin.me](https://tippin.me/) и бота _lntxbot_, о котором мы поговорим чуть позже, до сайтов наподобие [https://microlancer.io/](https://microlancer.io/), где можно выполнять простые задания в обмен на сатоши, и написания статей, открывающихся к просмотру после оплаты сатошиками на площадке [Y’alls](https://yalls.org/). Помимо этого, в зависимости от страны проживания вы можете воспользоваться такими сервисами, как [Lolli](https://www.lolli.com/), которые возвращают часть стоимости покупок в биткоинах.

Если вы уделите чуть больше времени и немного ресурсов, то, запустив собственную лайтнинг-ноду, вы сможете открывать каналы и сдавать их в аренду желающим осуществлять транзакции. На канале скоро выйдет видео о настройке лайтнинг-ноды, а пока при желании вы можете изучить ресурс [https://github.com/lightninglabs/pool](https://github.com/lightninglabs/pool).

Тем не менее, самыми простыми способами заработка сатоши является просмотр рекламы за небольшие вознаграждения внутри телеграм-бота @lntxbot и предоставление услуг взамен на оплату в сети лайтнинг.

---

## С чего начать?

Первым шагом во взаимодействии с любым “крипто-решением” всегда является выбор кошелька. Лайтнинг не стал исключением, и в первую очередь нам стоит определиться какой графический интерфейс выбрать для взаимодействия с сетью.

Для начинающих я бы порекомендовал обратиться к так называемым кастодиальным кошелькам — кошелькам, которые хранят ваши средства. Знаю, что многие сейчас вспомнят старое доброе высказывание “Не твои ключи — не твои биткоины”, и я полностью с вами согласен, но лайтнинг, будучи протоколом второго уровня, то есть надстройкой над протоколом Биткоин, еще сложнее в плане настройки. Поэтому начать с кастодиального решения отнюдь не зазорно. Вы всегда можете сменить подход как только вы убедитесь в собственных силах и запустите собственную ноду.

Примерами таких кошельков являются [Wallet of Satoshi](https://www.walletofsatoshi.com/), [Blue Wallet](https://bluewallet.io/) и многие другие. Подробнее о кошельках, поддерживающих лайтнинг читайте в этой статье:

[Lightning-кошельки](https://www.21ideas.org/theory-ln-lightning-wallets/)

Создав кошелек вам потребуется отправить на него немного биткоинов, после чего внутри приложения вы сможете конвертировать полученные биткоины в биткоины, предназначенные для сети лайтнинг. Разные приложения взаимодействуют с пользователем по разному, но, как правило, все они интуитивны и не должны вызвать никаких сложностей. В итоге вы сможете пользоваться вашими лайтнинг-биткоинами так же, как и в случае с обычными - можно создавать и оплачивать счета и взаимодействовать со всеми, кто принимает лайтнинг-оплату.

---

## Передача ценности в сети лайтнинг

Транзакции в сети лайтнинг проходят через специальные каналы и осуществляются посредством генерации и оплаты счетов. Чтобы оплатить тот или иной счет необходимо сканировать предложенный контрагентом QR-код или вставить ссылку на инвойс в свой кошелек.

| ![pic2](https://github.com/LightningTony/bitcoin-guide-pics/blob/main/practical/Zachem_nuzhna_set_lajtning/pictures/pic2.png) |
|:--:|
| LNURL1DP68GURN8GHJ7MRWW3UXYMM59E3K7MF0D3H82UNV9ACXZ7FLW4EK2UNWV9KK2025DAH8JH6VD9NKSARWD9HXWZFEG78 |

### Передача ценности в сети лайтнинг, не покидая Telegram

С развитием лайтнинг появилось множество сторонних сервисов, облегчающих взаимодействие с сетью. Одним из таких полезных решений стал Telegram-бот [@lntxbot](https://t.me/lntxbot). С его помощью можно пересылать сатоши другим пользователям популярного мессенджера, и даже благодарить/поддерживать сатошиками высказывания ваших собеседников в чатах, в которых установлен этот бот. Описание работы бота и все возможные команды доступны по команде /help. Более того, каждый пользователь Telegram автоматически имеет страничку с так называемым LNURL - специально сгенерированным адресом в сети лайтнинг. Просто введите [https://lntxbot.com/](https://lntxbot.com/@Tony_Lightning) и добавьте к этой ссылке юзернейм пользователя, например мой LNURL — [https://lntxbot.com/@Tony\_Lightning](https://lntxbot.com/@Tony_Lightning)

---

## И это все?

Сам протокол Биткоин и сеть лайтнинг, как решение второго уровня, стремительно развиваются. Мы постоянно видим новые решения по оптимизации протокола, улучшению пользовательского опыта и многого другого.. Количество сервисов, принимающих биткоин стремительно растет с каждым днем.

За последние 10+ лет Биткоин уже доказал, что никуда не денется — он функционировал практически без перебоев с самого запуска протокола в январе 2009 года. Изучить Биткоин и сопутствующие протоколы сейчас — все равно, что погрузиться в океан интернет-решений в нулевых. Быть первопроходцем нелегко, но и вознаграждение за любопытство и труд, как правило, не заставит себя ждать!

---

_Tony_
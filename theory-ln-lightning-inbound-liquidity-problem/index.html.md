 

Если вы хотите принимать платежи через лайтнинг или правильно балансировать каналы, у вашего узла должна быть достаточная входящая емкость. В этой статье описывается, что это такое и каковы практические способы ее получения.

<h1 id="%D0%BF%D1%80%D0%BE%D0%B1%D0%BB%D0%B5%D0%BC%D0%B0">Проблема</h1>

<figure class="kg-card kg-image-card"><img alt="" class="kg-image" loading="lazy" src="https://lh4.googleusercontent.com/ilaivtiYj8avBS2RGF5-jHnF-ROkE_FBWIcmiguNo9cOTh-yO_Y8AWQADl4zVlQoTHzuUsbzxBzN1sTCycnbgSQ4ytqTLAViy5jmi-7Vh5JPTz59p0ykt6f3cOF1PDuumHHyRvRC=s0"/></figure>

_Упрощенный пример. Левый график показывает каналы и их емкость - информацию, видимую публично. Правый график показывает, как балансы на самом деле распределены внутри каждого канала (недоступная публично информация) и направления движения средств. Из картинки слева может показаться, что узел E имеет лучшее соединение. Но на практике все его балансы локальны, у него нет входящей емкости, и он не может принимать или маршрутизировать платежи._  

Функционирование платежей в Lightning Network (LN) отличается от ончейн биткоин-транзакций. Моя [предыдущая статья](https://bitcoin-translated.ru/sources/bitcoin-abc/lightning-network/) описывает криптографическую магию, стоящую за LN, ниже приведены лишь некоторые практические моменты.  

*   Сеть лайтнинг состоит из двусторонних каналов, в которых и заблокированы монеты.
*   Общее количество биткоинов, заблокированных в канале, называется емкостью канала.
*   Сумма на вашей стороне канала называется локальным балансом. Сумма на стороне партнера по каналу называется удаленным балансом.
*   Когда вы открываете новый канал — весь ваш баланс является локальным (здесь мы опускаем двойные каналы и проталкивание сумм с целью упростить пояснение).
*   Емкость канала всегда остается неизменной (для простоты мы опускаем [сплайсинг](https://medium.com/muunwallet/splices-and-liquidity-in-the-lightning-network-1d4bd4bc7575)) и примерно равна сумме локального и удаленного балансов (из-за комиссий).
*   Когда вы платите - баланс перетекает с вашей стороны канала на удаленную сторону. Когда вы получаете платежи — наоборот.

Что приводит нас к одной из основных проблем:

_Для того чтобы получать платежи, ваш узел должен иметь достаточную входящую емкость: достаточное количество открытых каналов с достаточным удаленным балансом (иначе баланс не может перетекать на вашу сторону)._

Увеличить входящую емкость означает как-то получить каналы с большим удаленным балансом. А для маленьких новых узлов это может быть очень сложно. И если данная проблема вас не пугает, имеет место еще один аспект:

>  _Не каждая входящая емкость одинаково полезна. Канал от хорошо соединенного и сбалансированного узла соединит ваш узел с сотнями других узлов. Канал от нового непубличного узла — нет._

Недоумеваете, как получить достаточную входящую емкость? Не переживайте — есть способы!

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-1-%D1%82%D1%80%D0%B0%D1%82%D0%B0">Решение 1: Трата</h1>

Это — очевидное решение, но его необходимо упомянуть. Когда вы используете канал для траты монет, они списываются с локального баланса и добавляются к удаленному. Чем больше вы тратите — чем больше ваш удаленный баланс, тем больше входящая емкость. 

Конечно, такой подход не решает всех проблем для каждого. Но если у вас есть возможность платить через LN — используйте ее, и в будущем у вас будет меньше проблем с входящими платежами.

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-2-%D0%BF%D0%BE%D0%BF%D1%80%D0%BE%D1%81%D0%B8%D1%82%D1%8C-%D0%BE%D1%82%D0%BA%D1%80%D1%8B%D1%82%D1%8C-%D1%81-%D0%B2%D0%B0%D0%BC%D0%B8-%D0%B2%D1%85%D0%BE%D0%B4%D1%8F%D1%89%D0%B8%D0%B9-%D0%BA%D0%B0%D0%BD%D0%B0%D0%BB">Решение 2: Попросить открыть с вами входящий канал</h1>

<figure class="kg-card kg-image-card"><img alt="" class="kg-image" loading="lazy" src="https://lh6.googleusercontent.com/oLnNMiPnAqUAozHUpJ-_n8GmWOCBQ2K1klmPjRMK4TUbUcOJhNItjA7n1gQaPlsK7-X1wPBd43XOWajkne0k-oMt3Ien5jPW45e66eImkCpVEWQ7OWxEN4O1YvIfNRBJPxaj4s89=s0"/></figure>

Это, пожалуй, лучший вариант для большинства узлов: если вам нужна входящая емкость — запросите входящие каналы. Если вы мерчант — попросите своих клиентов, если вы знаете кого-то, кто держит полную ноду — попросите их.

Но, несомненно, самый простой способ - это использовать сервисы, которые занимаются открытием каналов. Перечислим некоторые из них:

1.   [Thor](https://medium.com/@bitrefill/2d6ffbad3906) - сервис от проекта [Bitrefill](https://www.bitrefill.com/), предлагающего продукты и услуги, которые предоставляют возможность платить криптовалютами за разнообразные сервисы. Они могут арендовать вам частный канал с емкостью от 0.003 до 0.16 BTC, который они обещают держать открытым как минимум 30 дней. В зависимости от вместимости он будет стоить от доллара и до более чем $20.
2.   [Y'alls](https://yalls.org/about/) - услуга от [Алекса Бошворта](https://twitter.com/alexbosworth), которая позволяет вам заплатить менее доллара за канал с входящей емкостью в 0.02 BTC. И хотя это может показаться дешевле, чем Bitrefill, имейте в виду, что Y'alls устанавливает более высокие, чем обычно, тарифы на маршрутизацию (которые придется платить вашим клиентам).
3.   [LightningTo.Me](https://lightningto.me/) - мой личный некоммерческий хобби-проект, который бесплатно откроет канал BTC 0.02 с вашим узлом. И да, он также не взимает плату за маршрутизацию. [Здесь](https://github.com/LightningTo-Me/manuals/blob/master/Channel_Request.md) вы можете найти ответы на некоторые часто задаваемые вопросы.
4.   [LNBig.com](https://lnbig.com/#/) - крупный провайдер ликвидности, который бесплатно откроет канал до 0.04 BTC. Их политика в отношении тарифов на маршрутизацию меняется довольно часто, так что обратите на это внимание.

Есть также узлы, которые обещают открыть канал с вашим узлом, если вы первым откроете канал с их узлом. Предлагаю обратить внимание на [WILL\_CONNECT\_BACK](https://1ml.com/node/03ee180e8ee07f1f9c9987d98b5d5decf6bad7d058bdd8be3ad97c8e0dd2cdc7ba) или [Lightning Power Users](https://lightningpowerusers.com/home/). Остерегайтесь, что это не всегда будет работать с нодами, на которых запущена c-lightning, которая разрешает только один канал между двумя узлами.

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-3-%D0%BA%D0%B0%D1%81%D1%82%D0%BE%D0%B4%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9-%D0%BE%D0%B1%D0%BC%D0%B5%D0%BD-%D0%BB%D0%B0%D0%B9%D1%82%D0%BD%D0%B8%D0%BD%D0%B3-%D0%B1%D0%B8%D1%82%D0%BA%D0%BE%D0%B8%D0%BD%D0%BE%D0%B2-%D0%BD%D0%B0-%D0%BE%D0%BD%D1%87%D0%B5%D0%B9%D0%BD-%D0%B1%D0%B8%D1%82%D0%BA%D0%BE%D0%B8%D0%BD%D1%8B">Решение 3: Кастодиальный обмен лайтнинг-биткоинов на ончейн-биткоины</h1>

Для некоторых это может показаться нелепым, но это действительно является одним из решений: вы можете обменять биткоины на биткоины. В каком-то смысле, это тоже форма траты: вы тратите лайтнинг-биткоины и получаете ончейн монеты взамен.

Я надеюсь, что достаточно скоро многие крупные биржи позволят осуществлять лайтнинг-депозиты, но на данный момент вариантов не так уж и много. Я упомяну некоторые из них: [zigzag.io](https://zigzag.io/), [fixedfloat.com](https://fixedfloat.com/), [sideshift.ai](https://sideshift.ai/), [southxchange.com](https://www.southxchange.com/), [btcduke.com](https://www.btcduke.com/?lang=en), [coinplaza.it](https://www.coinplaza.it/), [lightningconductor.net](https://lightningconductor.net/invoice).

Пожалуйста, имейте в виду, что услуги биржи не всегда надежны. Проведите собственное исследование и сразу же после осуществления сделки выведите свои монеты.

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-4-%D0%BE%D0%B1%D1%80%D0%B0%D1%82%D0%BD%D1%8B%D0%B5-%D0%BD%D0%B5%D0%BA%D0%B0%D1%81%D1%82%D0%BE%D0%B4%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D1%8B%D0%B5-%D1%81%D1%83%D0%B1%D0%BC%D0%B0%D1%80%D0%B8%D0%BD-%D1%81%D0%B2%D0%BE%D0%BF%D1%8B">Решение 4: Обратные некастодиальные субмарин-свопы.</h1>

Как и предыдущее решение, обратные некастодиальные субмарин-свопы реализуют обмен лайтнинг- (оффчейн) биткоинов на ончейн монеты. Но это решение лучше, чем предыдущее, так как оно не является кастодиальным (не требует доверия). На данный момент оно не очень удобно в использовании и больше ориентировано на разработчиков, поэтому я не буду в него углубляться. Пожалуйста, ознакомьтесь с [этим блог-постом](https://blog.lightning.engineering/posts/2019/03/20/loop.html) или перейдите непосредственно в [репозиторий github](https://github.com/lightninglabs/loop).

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-5-%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D1%82%D1%8C-%D0%BA%D0%B0%D1%81%D1%82%D0%BE%D0%B4%D0%B8%D0%B0%D0%BB%D1%8C%D0%BD%D0%BE%D0%B5-%D1%85%D1%80%D0%B0%D0%BD%D0%B8%D0%BB%D0%B8%D1%89%D0%B5">Решение 5: Использовать кастодиальное хранилище</h1>

Это еще более опасный способ, потому что он требует от вас доверия к услуге в течение длительного периода времени. Исследование каждой площадки здесь еще более важно, чем в предыдущем случае. По сути, эти услуги позволяют вам предоставить свои средства им на хранение и обещают вернуть их, когда они вам понадобятся.

В качестве примеров можно привести различные кошельки для хранения средств: [BlueWallet](https://bluewallet.io/),[ Wallet of Satoshi](https://www.walletofsatoshi.com/) or[ Bitlum](https://bitlum.io/). В данном случае все максимально просто: вы отправляете лайтнинг-биткоины с вашей ноды на их, освобождая локальный баланс вашей ноды.

_Но если вы достаточно креативны, вы можете воспользоваться и другими услугами. Например, вы можете послать себе щедрый донат через _[_tippin.me_](https://tippin.me/)_. Таким образом, вы будете хранить некоторую часть ваших средств на их узле._

<h1 id="%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B5-6-%D1%83%D0%B1%D0%B5%D0%B4%D0%B8%D1%82%D0%B5%D1%81%D1%8C-%D1%87%D1%82%D0%BE-%D0%B2%D0%B0%D1%88-%D1%83%D0%B7%D0%B5%D0%BB-%D0%B2%D1%81%D0%B5%D0%B3%D0%B4%D0%B0-%D0%B2-%D1%81%D0%B5%D1%82%D0%B8">Решение 6: Убедитесь, что ваш узел всегда в сети.</h1>

Если вы просто будете держать ваш узел всегда в режиме онлайн — вы, скорее всего, получите некоторую входящую емкость. Открывайте каналы на множестве хорошо обслуживаемых узлов (я был бы признателен, если бы [мой узел](https://1ml.com/node/03bb88ccc444534da7b5b64b4f7b15e1eccb18e102db0e400d4b9cfe93763aa26d) был одним из них), убедитесь, что ваш узел публично рекламирует свой IP-адрес, проверьте, что порты открыты, и настройте мониторинг, чтобы убедиться, что программное обеспечение LN работает круглосуточно, семь дней в неделю.

Во-первых, пользователям нравятся узлы с хоть каким-то подключением, которые всегда находятся в сети, потому что эти узлы с большей вероятностью будут получать платежи от своих пользователей. Во-вторых, некоторые узлы работают на автопилоте, и если вы находитесь в сети — вы можете настроить канал с этими узлами просто случайно.

<h1 id="%D0%B7%D0%B0%D0%BA%D0%BB%D1%8E%D1%87%D0%B5%D0%BD%D0%B8%D0%B5">Заключение</h1>

Принимать платежи с помощью лайтнинг сложнее, чем принимать ончейн платежи, но не отчаивайтесь, используйте некоторые из приведенных выше советов. Со временем ваш узел созреет и все заработает как швейцарские часы.

У вас есть комментарии? Я что-то забыл? Пожалуйста, не стесняйтесь поделиться своими мыслями! Давайте продолжим улучшать этот пост и поможем лайтнинг расти. О, и следите за обновлениями LightningTo.Me в [твиттере](https://twitter.com/LightningTo_Me)!
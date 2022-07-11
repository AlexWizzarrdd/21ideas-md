 >  Данный краткий гид по покупке биткоина подготовлен дружественным проектом [Биткоин-абстракцион](https://t.me/bitraction/342). 

<h1 id="%D0%BF%D1%80%D0%B5%D0%B4%D0%B8%D1%81%D0%BB%D0%BE%D0%B2%D0%B8%D0%B5">Предисловие</h1>

В силу сложившейся ситуации в стране я решил написать этот мануал по покупке биткоина для новичков и откинуть любые рассуждения о том, где и как лучше покупать и хранить биткоин, о минусах и плюсах разных вариантов, типах кошельков и тому подобном. В этом посте я опишу лишь кратчайший способ покупки биткоина с нулевыми навыками и опытом.

Я сам, основываясь на собственном опыте и личных знаниях, выбрал, на мой взгляд, наилучшие ресурсы с расчетом на то, чтобы этот мануал подошел даже людям далеким от биткоина. Так что этот материал вы можете скидывать своим родителям, братьям, сестрам и друзьям, которые просто хотят уберечь свои сбережения в обстановке свободного плавания (или падения) российской экономики.

_Примечание для опытных биткоинеров_: здесь не будет [multisignature хранилищ](https://www.21ideas.org/tag/multisig/), [p2p-сервисов](https://youtu.be/aZQ-9rZG0-w), [настроек нод](https://www.21ideas.org/practical-why-run-own-node-part-1/) и подобных комплексных топиков. Материал, как и сказано выше, описывает сбалансированный и кратчайший способ покупки биткоина в условиях экстренной ситуации в стране __для каждого__!

__ВАЖНО!__ Ниже я поясню причину выбора именно тех сервисов, которые будут описаны в этом гиде.

__Во-первых__, для хранения и перевода биткоинов я выбрал __Muun Wallet__, потому что он сочетает в себе простоту и функционал, а так же отвечает последним запросам в среде биткоина. Биткоин сегодня — это повышенная надежность и безотказность основной сети и транзакций в ней (далее __onchain__), а так же моментальные транзакции и _несправедливо низкие_ комиссии (с учетом быстроты и удобства) в сети второго уровня (далее __lightning__)

Поясню так же, что [Lightning](https://www.21ideas.org/theory-lightning-why-lightning/) использует сеть второго уровня для совершения быстрых платежей, но это всё ещё Биткоин. Это можно представить себе как бумажные деньги, подкрепленные золотом. Золото – это приоритет надежности, а бумажные деньги приоритезируют скорость и удобство. Золото — onchain, деньги — lightning. Выбор в пользу Muun Wallet был сделан из-за того, что кошелек визуально объединяет onchain и lightning счета в один общий счет и сам выполняет процессы под капотом в автоматизированном режиме. Именно поэтому он подойдет всем новичкам.

__Во-вторых: __Для покупки биткоина мы будем использовать обменники и агрегатор обменников. Сайт bestchange.ru уже долгое время является надежным агрегатором онлайн-обменников, где можно в кратчайшие сроки и по актуальному курсу купить биткоин. К тому же, можно найти обменники, которые не запрашивают KYC (проверку документов или карты), что является приоритетом для нас в данном материале. Как отличить обменники, требующие пройти KYC от тех, которые этого не делают, расскажу ниже.

__В третьих: __после покупки биткоина, возможно, вам захочется лучше изучить его устройство. Получить и расширить знания о биткоине с технической, экономической и философской сторон можно на сайте [21ideas.org](http://21ideas.org/). Это – самый полный русскоязычный портал с информацией о биткоине. Также советую начать с [этого](https://youtu.be/LrmhcaD6Cfg) и [этого](https://youtu.be/j9-4OnxOto8) видео.

<h1 id="%D0%BD%D0%B0%D1%81%D1%82%D1%80%D0%BE%D0%B9%D0%BA%D0%B0-%D0%B8-%D0%BF%D1%80%D0%B8%D0%BD%D1%86%D0%B8%D0%BF-%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D1%8B-muun-wallet">Настройка и принцип работы Muun Wallet</h1>

Ссылка для скачивания для iOS и Android: 

<figure class="kg-card kg-bookmark-card"><a class="kg-bookmark-container" href="https://www.muun.com"><div class="kg-bookmark-content"><div class="kg-bookmark-title">Muun - Bitcoin Wallet</div><div class="kg-bookmark-description">Muun is a self-custodial wallet for Android and iOS. Make fast and cheap payments. Keep your money safe.</div><div class="kg-bookmark-metadata"><img alt="" class="kg-bookmark-icon" src="https://www.muun.com/apple-touch-icon.png"/><span class="kg-bookmark-author">Bitcoin and Lightning Network</span></div></div><div class="kg-bookmark-thumbnail"><img alt="" src="https://muun.com/social-share.png"/></div></a></figure>

Скачиваем MuunWallet и запускаем клиент на своем устройстве. Кошелек нужен, чтобы сгенерировать свой уникальный публичный адрес, который будет использоваться для получения/хранения/отправки биткоина.

<figure class="kg-card kg-image-card kg-card-hascaption"><img alt="" class="kg-image" loading="lazy" src="https://telegra.ph/file/33198e2abcb4d57809b01.png"/><figcaption>1. Стартовый экран; 2. Главный экран кошелька; 3. Создание бэкапа.</figcaption></figure>

После запуска нажимаем «_Create a new wallet_». Кошелек попросит вас создать пин-код для входа в приложение, после чего пустит на главный экран с балансом.

Первое что __ОБЯЗАТЕЛЬНО__ нужно сделать перед продолжением работы – это нажать на «_Back up your wallet_» и пройти процедуру создания бэкапа кошелька.

Для чего это нужно:  
Ваши биткоины не хранятся непосредственно на устройстве. Вся работа сети устроена таким образом, что вы имеете публичный адрес, которым делитесь с другими людьми для получения монет, но для отправки транзакций вам также необходим &nbsp;приватный ключ, которым приложение подписывает каждую вашу транзакцию. Можно сказать, это ваша электронная подпись, защищенная криптографией. Ваши средства хранятся в сети, а доступ к ним можно получить ТОЛЬКО имея этот приватный ключ. Этот ключ хранится в устройстве и надежно зашифрован, но если вы вдруг потеряете доступ к самому устройству (потеряете/сломаете телефон), то с помощью данного ключа вы сможете восстановить доступ к деньгам.

Именно поэтому отнеситесь к этому этапу настройки с максимальным вниманием и осторожностью! От этого этапа зависит сохранность ваших средств. Вы вступаете на дорогу личного финансового суверенитета, поэтому такая защита необходима, ведь никакой банк больше не отвечает за ваши деньги. Они полностью под вашим контролем и теперь вы в ответе за их безопасность. 

На экране создания бэкапа, как показано на скриншоте номер 3 выше, вы видите 3 этапа процедуры. Она занимает 5 минут.

1.   Первый этап включает в себя указание вашей электронной почты, чтобы Muun в случае чего смог отправить вам указания по восстановлению средств. Его можно пропустить, если вы не хотите делиться своими данными.
2.   Второй этап является самым важным! Приложение сгенерирует специальный код. Запишите его на физический носитель (на листок бумаги, в дневник и т.п.) и надежно сохраните. Храните этот код в укромном месте, о котором знаете только вы. __НЕ ЗАПИСЫВАЙТЕ__ этот код в заметки на телефоне или компьютере, это небезопасно! Это ваш единственный способ восстановить средства в случае потери доступа к ним. Любой недоброжелатель, к которому попадет этот код, может восстановить ваши средства на своем устройстве и перевести их куда угодно. Будьте осторожны!
3.   Третий этап требует от вас сохранить так называемый _Recovery _файл. Данные на нем зашифрованы и не ведут напрямую к вашим средствам, поэтому Muun разрешает сохранять его к себе в файлы на устройство, в iCloud или Google Drive. Сделайте это, чтобы иметь возможность вывести свои средства даже без использования Muun в случае, если по каким-либо причинам приложение перестанет существовать. Это делается в комбинации с вашим кодом восстановления из второго этапа, так что сам по себе этот файл бесполезен для мошенников. В файле есть полная инструкция, на данный момент она вам не нужна.

Отлично! После создания бэкапа вы готовы принимать и отправлять биткоины со своего кошелька. Нажмите кнопку «__Receive__» на главном экране, чтобы увидеть свой адрес, которым вы можете делиться с другими людьми для получения монет.

<figure class="kg-card kg-image-card kg-card-hascaption"><img alt="" class="kg-image" loading="lazy" src="https://telegra.ph/file/f21a758f20a9041f828b6.png"/><figcaption>При каждом следующем входе в приложение адреса будут меняться. Это сделано для повышения анонимности. Все старые адреса будут работать, не переживайте.</figcaption></figure>

На экране получения мы видим вкладки Bitcoin и Lightning. Это именно то, о чем я говорил вам в начале материала. На вкладке Bitcoin мы получаем QR код, который содержит в себе ваш адрес, написанный прямо под ним. Вы можете тапнуть по нему и скопировать адрес. В опции «Amount» вы можете указать сумму, которую собираетесь запросить у отправителя.

Важный параметр, который стоит запомнить — биткоин адреса. В «Address type» должен быть выставлен _Segwit_ адрес, но если в одном из редких случаев возникает проблема с получением, выберите параметр _Legacy_. Не буду сейчас подробно рассказывать о разнице между этими форматами, просто скажу, что по возможности используйте Segwit. Это новый тип адресов, при использовании которого комисси ниже, чем в случае с адресами Legacy.

На вкладке Lightning мы видим примерно то же самое в плане устройства. Вы не можете получить onchain-биткоины на адрес lightning или наоборот. Lightning-адрес временный, о чем говорит нам время истечения внизу экрана. Такой тип оплаты больше подходит для моментальных платежей, к примеру: вживую другому человеку, в кафе и т.д. (если, конечно, они принимают такой вид оплаты). Но для покупки и хранения ваших биткоинов мы будем использовать только onchain адрес.

<h1 id="%D0%BF%D0%BE%D0%BA%D1%83%D0%BF%D0%BA%D0%B0-%D0%B1%D0%B8%D1%82%D0%BA%D0%BE%D0%B8%D0%BD%D0%B0">Покупка биткоина</h1>

После настройки вашего кошелька нам остается только купить биткоин. Для этого будем использовать обменники с сайта [bestchange](https://www.bestchange.ru).

Bestchange – это агрегатор обменников, по аналогии с AviaSales, который не продает билеты напрямую, но показывает вам в удобном виде предложения других сервисов. Я выбрал именно этот ресурс, потому что он быстрый, удобный и, что немаловажно, выгодный. Сейчас из-за санкций многие централизованные сервисы по покупке биткоина перестают работать, поэтому важно выбрать именно тот, который останется актуальным на момент прочтения этого материала в будущем.

Все обменники на bestchange проверены, так что можно не бояться, что где-то вас обманут. __Но__ есть несколько параметров, по которым стоит выбирать подходящий.

<figure class="kg-card kg-image-card kg-card-hascaption"><img alt="" class="kg-image" loading="lazy" src="https://telegra.ph/file/c591ac09de5003cacec8c.png"/><figcaption>Главная страница bestchange.ru</figcaption></figure>

На сайте достаточно простая навигация, если знать какой параметр за что отвечает. Давайте разбираться.

Слева есть 2 зеленых столбца. В левом вы выбираете способ оплаты. Например, у меня рубли на карте Сбера. Значит выбираю Сбер. В правом столбце вы выбираете что будете покупать. В нашем случае это биткоин (BTC). Он занимает первое место в столбце.

После выбора этих двух параметров сайт автоматически обновляется и выдает вам релевантные обменники в центральной части экрана. У сайта есть короткое видео о том, как он работает. Вы можете посмотреть его [тут](https://youtu.be/hgx0IScTiQM). Но я сейчас объясню только основные моменты, необходимые нам для покупки.

1.   Над списком обмена есть кнопка «Калькулятор»; нажмите на неё и введите сумму, которую планируете обменять на биткоин. Нажмите «Рассчитать» справа и сайт снова обновится, выдав те обменники, которые могут продать вам биткоин на эту сумму.
2.   Приложение стандартно сортирует все обменники по цене ВТС от меньшей к большей.
3.   В самой правой колонке указано количество отрицательных и положительных отзывов об обменнике. Если у обменника есть хотя бы несколько отрицательных отзывов, __советую выбрать другой__.
4.   Рядом с названиями обменников, как это показано на скриншоте выше, располагаются зеленые иконки. Если вы не хотите проходить процедуры подтверждения документов и карты, то __воздержитесь__ от покупки биткоина на подобных площадках. Вы можете навести указатель на иконки рядом с названием, и обменник покажет её значение в выпадающем сообщении.

<figure class="kg-card kg-image-card kg-card-hascaption"><img alt="" class="kg-image" loading="lazy" src="https://telegra.ph/file/7c23035ba8caf7f6ab144.png"/><figcaption>К примеру, вот данный обменник не имеет иконки ключа или банковской карты, а значит не потребует от вас регистрации или подтверждения карты.</figcaption></figure>

После выбора щелкаете на обменник и переходите на его сайт. Я не знаю, что вы выбрали. Поэтому дальше опишу стандартные действия для большинства случаев и каких действий не стоит бояться:

При обмене средств на сайтах без регистрации/проверки карты вы просто должны будете ввести свой биткоин-адрес, который мы с вами получили в MuunWallet, а также ввести номер своей карты, с которой будет производиться оплата. Возможно попросят внести email-адрес, на который после придет информация о сделке. Если обменник будет ругаться на биткоин-адрес, просто поменяйте его на Legacy-адрес в Muun и вставьте новый адрес в нужное поле. SegWit-адреса обычно начинаются с "bc1", а Legacy-адреса начинаются с цифры 1 или 3.

После заполнения информации для обмена, на следующей странице вам дадут номер сделки и заморозят курс на время её совершения. Далее обычно дают реквизиты карты, на которую необходимо перевести деньги. Делайте это внимательно и вводите точную сумму до последнего знака.

После оплаты нажимаете на сайте кнопку «Оплатил» и ждете проведения операции и поступления денег на ваш кошелек Muun. Операция может занять до 30 минут и дело не только в работе обменника. Сеть Биткоин должна подтвердить транзакцию, совершенную обменником. При высоких нагрузках в сети это занимает некоторое время. В любом случае не закрывайте окно сделки, пока не увидите поступившие средства в кошельке Muun. Кстати, когда средства отобразятся, рядом с балансом сначала появится желтая иконка часов. Не переживайте, она исчезнет через несколько минут, когда транзакция подтвердится. Механизм работы сети Биткоин отличается от функционирования традиционной системы, я не будем сейчас вдаваться в подробности, лишь сообщу, что транзакции с часиками сбоку вполне достаточно, чтобы быть спокойным, что средства зачислены.

Я не рекомендую использовать [сервисы, которые просят вас подтвердить вашу личность](https://www.21ideas.org/privacy-no-kyc/), но можно использовать сервисы с подтверждением банковской карты. Процедура подтверждения на таких сайтах заключается в отправке фотографии карты на фоне сделки. Закройте все данные карты, кроме номера и имени, и загрузите фото на сервис. Этого действия так же не стоит бояться, если вы выбрали проверенный обменник из списка на bestchange.

<h1 id="%D0%B2-%D0%B7%D0%B0%D0%B2%D0%B5%D1%80%D1%88%D0%B5%D0%BD%D0%B8%D0%B5">В завершение</h1>

1.   Никогда __не__ __показывайте__ код восстановления, который вы записали на бумагу при настройке MuunWallet. В этой фразе заключается полный контроль над вашим кошельком и единственная возможность его восстановить в случае утраты доступа.
2.   Старайтесь обходить сервисы с KYC (подтверждение личности). Биткоин — это ваша собственность. Единственная собственность, которую никто не сможет у вас отнять. Где, сколько и как вы хотите хранить свою собственность – дело ваше и только ваше. Биткоин это — личностный суверенитет. [Суверенитет посредством математики](https://www.21ideas.org/book-stm/).
3.   Если вы хотите пополнить знания о биткоине, рекомендую вам посетить сайт [https://www.21ideas.org](https://www.21ideas.org/) и Telegram каналы: <https://t.me/bitcoin21ideas&gt;&gt;&gt; и &lt;&lt;&lt;FLOATING LINK: https://t.me/bitraction>
4.   Если у вас остались вопросы по данному материалу, прошу задать их у нас в чате <https://t.me/bitractionchat&gt;&gt;&gt; или в комментариях к посту: &lt;&lt;&lt;FLOATING LINK: https://t.me/bitraction/342>.
5.   Больше информации о том, зачем и как самостоятельно хранить биткоин, можно найти [здесь](https://www.21ideas.org/practical/).

__Исправим деньги — исправим мир!__
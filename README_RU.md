# White Paper Nousplatform

Платформа и протокол для создания токенизированных инвестиционных фондов на блокчейне.

Авторы: Анатолий Островский, Вячеслав Пустовой

https://nousplatform.com

Дата последнего редактирования: 10.07.2017

## 1. Предисловие

С появлением криптовалют и ICO, правила игры на финансовых рынках меняются с огромной скоростью. Трейдеры и инвесторы нуждаются в новых технологиях, более доверительных, прозрачных, и главное простых для обеих сторон. С развитием блокчейна стало возможным то, что еще пару лет назад казалось фантастикой. Простым инвесторам стали доступны такие инструменты инвестирования, как криптовалюты и инвестиции в стартапы на ранних стадиях (ICO) с возможностью в любой момент продать свои активы или обменять на другие. Такие возможности инвестирования очень привлекательны и удобны, так как не требуют затяжных бюрократических процедур, уплаты высоких комиссий и минимальных порогов входа. Любой желающий может приобрести актив любой компании, выпустившей свои токены за любую сумму, заплатив лишь небольшую комиссию.

На фоне открывшихся возможностей все больше растет спрос на создание инвестиционных фондов для управления портфелями токенизированных активов и криптовалют. На фоне изменений законодательной базы в скором будущем институциональные игроки также займут нишу на этом рынке. Со временем инвестиции в токенизированные активы заменят привычные всем инвестиции в акции, фьючерсы, опционы и т.д., так как эти инструменты также возможно будет токенизировать, привязав их эмиссию к выпуску новых токенов. Уже сейчас мы видим развитие стартапов, которые пытаются токенизировать золото и другие металлы, как только это произойдет, то при помощи токенов станет возможным продавать и покупать любые виды активов в цифровом формате, что выведет инвестиционные фонды на новый этап развития.

В этом документе описан новый подход к созданию фондов, который позволяет внедрять блокчейн технологию в инвестиционную среду, и решать такие проблемы, как привлечение капитала, прозрачность деятельности фондов, децентрализованное хранение долевых активов инвесторов, высокая ликвидность, отсутствие посредников и многое другое.

### 2.1 Основные проблемы индустрии

К сожалению на сегодняшний день простому обывателю очень тяжело воспользоваться услугами инвестиционного фонда. Мы обобщили основные препятствия с которыми инвестор сталкивается, пытаясь воспользоваться услугами фонда.

* Прозрачность отчетности фонда, гарантия, что статистика не подверглась манипуляциям со стороны менеджеров фонда

* Доверие к банку или брокеру, в котором фонд держит свои активы

* Высокий порог входа, высокие комиссии при переводе средств

* Привязка к определенной валюте и потеря при конвертации, так как нет возможности свободно купить валюту на межбанковском рынке, приходится платить банку большую комиссию за конвертацию

* Блокировка средств фондом на минимальный период, что делает актив инвестора абсолютно неликвидным

* Отсутствие сравнительной статистики фондов единого формата

* Языковые барьеры, сложная отчетность, непонятная простому обывателю терминология

* Сложности в приобретение ETF индексов, так как нужно переводить средства на разные биржи

* Слабые возможности диверсификации портфелей, из за практической невозможности участия одновременно в нескольких фондах исходя из вышеперечисленных причин

### 2.2 Рынки

Охват рынка, где может применяться протокол и платформа огромен и многообразен. Мы оцениваем его минимум в $10 трлн. Одна лишь компания BlackRock, Inc<sup>1</sup> имеет в управлении $5.5 трлн. активов. Существует также большое количество хедж фондов<sup>2</sup>, инвестиционных банков и компаний<sup>3</sup>, а также семейных фондов, частных фондов, венчурных фондов. Переход фондов в будущем на блокчейн очевиден, так как это решает ряд проблем и улучшает различные показатели.

## 3. Ноус Протокол

*Краткое описание: протокол позволяет быстро создать фонды различного типа для управления блокчейн активами. Фонд полностью оснащен всеми нужными инструментами для работы с портфелями и управлением взаиморасчетов с инвесторами. В качестве измерения капитализации фонда используются ноус токены, которые позволяют инвестору купить или продать свою долю в фонде. Основные преимущества для открытых фондов является то, что выплата инвестору может происходить из резервных ноус токенов, которые фонд может держать, как актив своего инвестиционного портфеля, в этом случае фонду не надо закрывать другие позиции, чтобы рассчитаться с инвестором. Такой механизм будет очень позитивно влиять на динамику развития фонда, увеличивая его ликвидность.*

*Протокол позволяет также создавать закрытые фонды, которые в дальнейшем смогут торговать своим индексом (ETF) на любых криптовалютных биржах. Такой фонд может проводить ICO на платформе для привлечения первоначальных инвестиций.*

### 3.1 Какие проблемы решает платформа для менеджеров фонда

Менеджеры фонда получает полный набор инструментов для управления фондом и взаимодействия с инвесторами. Основные элементы взаимодействия регулируются при помощи смарт контрактов с открытым кодом, что делает фонд открытым и прозрачным, а соответственно более привлекательным для инвестора. Взаиморасчет с инвестором происходит при помощи смарт контракта который регулирует покупку или продажу части капитализации фонда, используя ноус токены.

При создании нового фонда формируется смарт контракт, который публикуется  его создателем при помощи ноус протокола на блокчейне. В смарт контракте прописаны параметры фонда, которые делятся на изменяемые и неизменяемые. Например параметры: дата создания фонда, начальный капитал, создатель фонда и т.д. не могут быть изменены после публикации контракта, а параметр минимальное время инвестирования может быть изменяемым. Создатель контракта с помощью ключа может изменить определенный параметр фонда, в таком случае новые правила будут действовать только для новых инвесторов, так как поменять правила задним числом будет физически невозможно. Такой подход обеспечит честные правила игры для обеих сторон и обезопасит инвесторов от манипуляций со стороны менеджеров фонда. Смарт контракт фонда также делегирует часть полномочий ноус смарт контракту, который в свою очередь имеет право использовать определенные доверительные функции, такие как проверка на владение активами, записи о состоянии инвестиционного портфеля, идентификация менеджеров фонда, расчет уровня доверия, и многое другое. Ноус смарт контракт также может добавлять сторонних эскроу контрагентов для дополнительного функционала.

Платформа ноус сама по себе является мощным инструментом по привлечению потенциальных инвесторов и созданию инвестиционного комьюнити, соответственно все фонды созданные на платформе автоматически попадают в поле зрения большого количества пользователей.


### 3.2 Какие преимущества дает платформа для инвесторов

Инвестор может в любое время принять участие в любом фонде, купив часть его капитализации за ноус токены. Приобрести ноус токены можно в свободном доступе на на крипто биржах. Сам токен ERC20 имеет все преимущества связанные с Ethereum, например использование единого кошелька для ERC20 токенов. Если инвестор хочет зафиксировать прибыль или часть прибыли, он продает часть капитализации фонда и получает обратно ноус токены по фиксированному на момент сделки курсу.

Инвестор может использовать сразу несколько фондов с различными портфелями для диверсификации рисков. Решение об участии в фонде принимается на основе анализа статистики фонда, зафиксированной на блокчейне и полностью исключающую манипуляции. Смарт Контракт создает с заданной периодичностью снапшоты инвестиционного портфеля каждого фонда и фиксирует их в блокчейне. Статистику можно посмотреть в любое время в личном кабинете, а сам код смарт контракта является открытым и общедоступным.

Инвестор в своем личном кабинете можете проанализировать деятельность любого фонда. Статистика фонда формируется по данным сделанных снапшотов, из которых видны такие данные, как доходность фонда в заданный промежуток времени, изменение активов в портфеле, добавление новых активов, индекс ликвидности, количество ноус токенов в резерве, личный капитал фонда от общего портфеля и тд.

Платформа будет также обладать инструментами для анализа и оценки фондов по различным статистическим данными, аналитические отчеты будут доступны любому пользователю.

Основные преимущества для инвесторов - это простота, прозрачность, возможность диверсификации, быстрый ввод/вывод средств, отсутствие бюрократии, заранее известные правила для обеих сторон, исключение любых манипуляций, отсутствие минимальных порогов входа.

В наши дальнейшие планы входит создание мерчанта на платформе ноус, что позволит инвесторам расплачиваться за товары и услуги, используя фондовые доли, то есть активы будут всегда находиться в фондах и использоваться только при надобности. Такой подход на наш взгляд может привести к новому виду торговых взаимоотношений между покупателем и продавцом, где деньги, как условная единица больше не понадобятся, экономика может перейти на токенизированный бартер.

##### *Пример 1*

Предположим Боб приобрел доли фонда, который занимается инвестициями в солнечную энергию и имеет в своих активах токены компаний, на которые раз в квартал начисляются дивиденды от проданной ими электроэнергии. Получив дивиденды на токены, фонд выплачивает их своим инвесторам. Соответственно Боб раз в квартал получает дивиденды на свою долю в фонде. Далее у Боба возникает потребность расплатиться за товар в магазине, он настраивает на платформе активы, которые готов потратить на оплату товара (в данном случае это один актив). Мерчант продает часть долей Боба фонду на нужную сумму и оплачивает товар.

Что произошло в данном случае? Для Боба это выглядит так, как будто он купил товар за часть электроэнергии, которая ему принадлежала, а для магазина это обычная транзакция. Конечно все это возможно при условии, что фонд имеет достаточный запас ноус токенов для мгновенных операций с инвестором, но как мы писали выше, фонд заинтересован иметь такой резерв для поддержания ликвидности. Сам магазин должен принимать ноус токены в качестве средства расчетов чтобы избежать подключения провайдера ликвидности и дополнительных комиссий, или задействовать более инновационные технологии, такие как протокол bancor.

## 4. Типы фондов

На первом этапе развития платформы мы планируем поддержку пяти типов фондов. Это смешанные фонды открытого и закрытого типа, венчурные фонды, благотворительные фонды и семейные фонды. В дальнейшем протокол ноус может быть расширен на поддержание более сложных форм фондов.

### 4.1 Фонд открытого типа (open-end)

Такой фонд продает и покупает собственные доли в любой момент времени. Инвестор посылает фонду свои средства в виде ноус токенов и получает взамен долю фонда, токенизированный инвестиционный пай, который может в любой момент вернуть и получить вложенные средства обратно по курсу оценки фондовой капитализации на момент выкупа. Такой подход позволяет фонду неограниченно наращивать собственную капитализацию, а инвестору иметь гарантированно ликвидный актив, который можно продать в любой момент. Фонд устанавливает комиссию за продажу или выкуп долей, что является его прямой прибылью.

### 4.2 Фонд закрытого типа (closed-end)

Фонд такого типа может привлечь инвестиции только один раз, после чего на полученные средства выпускается определенное фиксированное количество токенов. Токены распределяются между инвесторами в зависимости от вложенных средств. Далее фонд выводит свой токен на биржу, где он продается и покупается по рыночной цене, как ETF индекс. Фонд выплачивает всем владельцам токенов дивиденды от прибыли в назначенное время. На платформе ноус, фонды закрытого типа получают возможность проводить ICO (initial coin offering) для получения средств в управление,  представляя свой концепт сообществу инвесторов, использующих платформу.

Такой подход сможет привлечь фонду потенциальных инвесторов, а пользователям платформы даст выбор для диверсификации портфелей в закрытых фондах.

### 4.3 Венчурный Фонд 2.0

Для привлечение средств в стартапы или готовые бизнесы можно создать на платформе ноус венчурный фонд. Отличие такого фонда будет являться открытая система голосований, где сами инвесторы принимают решение об участии в том или ином стартапе. Решение принимается путем голосования каждого инвестора имеющего долю фонда. Такой фонд имеет особую экосистему, поэтому мы называем его более продвинутым фондом второго поколения.

##### *Пример венчурного фонда*

После проведения ICO поступившие средства инвесторов остаются заблокированы смарт контрактом и разблокируются только после открытого голосования. Предположим у фонда есть $10 миллионов, и менеджеры решают проинвестировать в стартап "Х" $500k, в этом случае они выставляют на голосование разблокировку $500k, и каждый инвестор может проголосовать при помощи смарт контракта за или против, оценив все шансы и риски стартапа. Если по регламенту набирается нужное количество голосов, то средства разблокируются для инвестирования. Преимущество такого фонда заключается в том, что каждый участник имеет свой вес в голосовании, например, если Боб имеет 10 долей, а Джон 2 доли, то голос Боба в 5 раз сильнее голоса Джона.

### 4.4 Благотворительный фонд

На ноус платформе можно создавать не только инвестиционные фонды, но и благотворительные. Основное преимущество благотворительного фонда на блокчейне является его прозрачность перед людьми, которые совершают пожертвования. Через ноус протокол можно контролировать деятельность благотворительного фонда, просматривать в открытом доступе кому и в каком размере была оказана помощь, и сколько средств было затрачено на оперативные расходы. Благотворительный фонд не имеющий границ способен привлекать пожертвования со всего мира. Любой владелец ноус токенов сможет сделать пожертвование в любой фонд, независимо от его местоположения.

### 4.5 Семейный фонд

Это также популярный тип фонда, когда родственники назначают управляющего деньгами семьи. Такой фонд не имеет публичной статистики. Отчеты видны лишь участникам фонда. В таком фонде можно также применять функцию открытого голосования с разблокировкой средств по принципу венчурного фонда.

Фонд может состоять и из одного человека, который может управлять своими средствами и пользоваться всеми преимуществами платформы. В таком случае 100% долей принадлежат одному человеку. Семейный фонд имеет еще одну интересную функцию, это управление наследством, когда активы одного родственника переходят другому, используя механизм смены владельца смарт контракта фонда.

## 5. Структура ноус экосистемы  

Техническая документация о возможностях системы будет предоставлена в отдельном документе. В этом документе мы предоставим краткий обзор компонентов.

Схема взаимодействия компонентов системы

![схема](https://nousplatform.com/assets/uploads/2017/07/nous-protocol-bg.png)

### 5.1 Ноус протокол
Это протокол с открытым кодом, разработкой которого занимается некоммерческая организация Nous Foundation. Протокол публикуется в открытом доступе и лицензирован под  [GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.en.html)

Протокол взаимодействует со смарт контрактами и имеет набор функций

Любой желающий может использовать протокол для создания собственного фонда. Изначально будет предоставлено решение с использованием библиотеки на Javascript, и в дальнейшем добавление остальных популярных языков программирования.

### 5.2 Ноус смарт контракт
Также является открытым кодом в рамках Nous Foundation и лицензирован под  [GNU Lesser General Public License v3.0](https://www.gnu.org/licenses/lgpl-3.0.en.html)

Смарт контракт исполняет доверительные методы внутри фондового контракта, такие как проверка на владение активами, записи о состоянии инвестиционного портфеля, идентификация менеджеров фонда, расчет уровня доверия, добавление сторонних эскроу контрагентов и т.д.

### 5.3 Фондовый смарт контракт
Создается и публикуется динамически через ноус протокол и имеет основные функции по управлению фондом, такие как долевое участие, выкуп долей, распределение токенов между инвесторами и многое другое.

### 5.4 Ноус кошелек
Кошелек является также открытым кодом и используется для хранения ноус токенов. При помощи кошелька также можно производить оплату и инвестировать токены в фонды.

### 5.5 Ноус Платформа
Коммерческая платформа для взаимодействия фондов и инвесторов. В нее входят личные кабинеты, статистика, кошельки, списки фондов и их предназначение. Для инвесторов платформа является решением под ключ для управления своими средствами.

Фонды также получают удобный интерфейс для работы и площадку по привлечению потенциальных инвесторов.

## 5. Платформа Ноус
Платформа представляет собой веб интерфейс, который взаимодействует с клиентским протоколом ноус, а также с API, которая в свою очередь взаимодействует с ноус смарт контрактом и базой данных

#### 5.1 Роли
Основные участники процесса разделяются на 5 групп
1. Создатель фонда (главный менеджер)
2. Менеджер фонда
3. Представляющий агент
4. Инвестор
5. Заверитель

#### 5.2 Функционал для менеджеров  
1. Главный менеджер регистрируется на платформе и подтверждает свои данные посредством двойной аутентификации. После процесса регистрации менеджер создает ноус кошелек на блокчейне и сохраняет себе приватный ключ. Адрес кошелька будет далее использоваться для публикации фондовых смарт контрактов. Далее менеджер пополняет кошелек ноус токенами для работы с блокчейном. Сам блокчейн берет небольшую комиссию за любые операции, связанные с записью информации, поэтому менеджеру нужны небольшие средства, например, чтобы опубликовать фондовый смарт контракт.

2. Главный менеджер создает фонд, вводит данные фонда, тип фонда, адреса кошельков менеджеров фонда. После чего ноус протокол публикует от имени главного менеджера смарт контракт на блокчейне с готовыми настройками. В смарт контракт вносятся также адреса смарт контрактов заверителей для использования различных трастовых функций.

3. Следующий шаг это добавление и верификация кошельков для формирования портфеля. Верификация нужна для того, чтобы фонд мог доказать, что активы инвесторов будут храниться именно на этих кошельках, а также подтвердить наличие или отсутствие собственного капитала управляющих менеджеров. Ноус протокол будет использовать различные способы верификации в зависимости от специфики блокчейна, на котором находится кошелек. Самый простой способ верификации, это пересылка микро сумм или OP_RETURN транзакций на предложенный ноус протоколом адрес, если транзакция прошла успешно, то протокол верифицирует кошелек фонда в смарт контракте.

4. Фиксация собственного начального капитала фонда, это один из важнейших аспектов, так как очень важно понимать, особенно для хедж фондов, какими собственными средствами рискуют менеджеры фонда. В момент верификации кошелька протокол считывает баланс и записывает его в смарт контракт, как начальный капитал фонда.

5. Публикация статистики. Ноус протокол с периодичностью в один день считывает с верифицированных кошельков балансы и транзакции, и записывает их через ноус смарт контракт в смарт контракт фонда. Статистика фонда доступна менеджерам фонда для аналитики.

6. Публикация фонда. Менеджеры фонда могут использовать ноус платформу для привлечения инвесторов. Фонд добавляется в рейтинги платформы, что является наиболее мощным маркетинговым инструментом по привлечению новых инвесторов.

7. Закрытые фонды могут использовать функционал ноус протокола для проведения ICO, то есть привлекать начальный капитал и выпускать собственные ETF токены. После создания фонда, менеджер может опубликовать дополнительный смарт контракт для проведения ICO, который коммуницирует с основным фондовым контрактом и контролирует распределение токенов.

8. Распределение ролей. Главный менеджер может распределять роли менеджеров внутри фондового смарт контракта, тем самым выдавать разрешение или блокировать доступ к различным функциям.


#### 5.3 Функционал для инвесторов
1. Инвестор регистрируется на платформе и получает личный кабинет. После чего проходит верификацию и получает собственный ноус кошелек, который пополняет ноус токенами.

2. Инвестор может просмотреть на платформе рейтинг и статистику, каждого фонда и принять решение об инвестировании. Фонды разбиваются на категории и типы. Инвестор может проанализировать деятельность фонда за любой промежуток времени.

3. Ноус протокол формирует трастовый уровень фонда, это измерительная единица, которая будет принимать значения в зависимости от различных факторов, связанных с деятельностью фонда. Это позволит инвесторам принимать более взвешенные решения.

4. Инвестор может покупать и продавать доли фонды. Участие в фонде обеспечивается путем приобретения долей фонда за ноус токены. Фиксация прибыли происходит за счет выкупа фондом собственных долей у инвестора за ноус токены. В закрытых фондах используется другой подход, см. пункт 6.

5. Безопасное хранение активов. Все активы приобретенные у фондов созданных ноус протоколом, хранятся в холодном кошельке, доступ к которому осуществляется только через приватный ключ, хранящийся у инвестора. Для хранения активов достаточно иметь один адрес кошелька.

6. Участие в ICO. Инвестор может заранее выкупить доли закрытого фонда, до того, как они попадут на биржу.

#### 5.4 Представляющий агент
Представляющий агент, это независимый партнер фонда, который занимается привлечением нового капитала в фонд и имеет определенную комиссию за проделанную работу. Протокол будет поддерживать функционал взаиморасчетов между фондом и представляющим агентом. При записи нового инвестора в фонд, протокол прописывает также адрес представляющего агента, если таковой имеется.

#### 5.5 Заверители
Основным заверителем является ноус смарт контракт, который отвечает за создание снапшотов балансов портфелей, присвоение фонду уровня доверия и так далее. То есть доверенный сервис, который имеет право осуществлять определенные действия с фондовым смарт контрактом

Также заверителями могут являться любые сторонние сервисы и разработчики, которые дополнят функционал смарт контракта. Ноус платформа может проводить голосования среди владельцев фондов по добавлению новых заверителей в смарт контракт фонда, и если решение принимается, то происходит добавление нового функционала и адресов смарт контрактов заверителей, имеющих доступ к этому функционалу.

##### *Пример 1*
Предположим существует сервис 'X', который занимается идентификацией пользователей по отпечаткам пальца или форме лица на блокчейне (уже сейчас мы наблюдаем за созданием таких сервисов<sup>4</sup>). Если фонд хочет верифицировать менеджера через сервис 'X', он разрешает смарт контракту сервиса внести изменения в смарт контракт фонда.

##### *Пример 2*
Сервис 'Y', организация осуществляющая контроль над фондами в зависимости от юрисдикции получает доступ к определенным функциям фондового смарт контракта для проведения аудита или блокировки деятельности фонда в случае нарушения законодательства или других причин.

##### *Пример 3*
Сервис 'Z', независимая организация в которую инвесторы могут подать жалобу на деятельность фонда, но не имеющая возможность влиять на работу фонда, может получить доступ для публикации рейтинга жалоб и решений конфликтов в смарт контракт фонда.  

Цель ноус протокола обеспечить максимальную простоту и удобство по интеграции сторонних сервисов и разработчиков.

## 6. Ноус токен
Ноус токен является универсальной валютой, при помощи которой, инвесторы смогут взаимодействовать с фондами. Ценность такой валюты очень велика, так как охватывает огромный рынок в триллионы долларов США. Токен будет иметь стандарт ERC20 и называться NOUS.

Основные применения ноус токенов:
1. Приобретение долей открытых фондов
2. Участие в ICO закрытых фондов
3. Выплаты дивидендов закрытых фондов
4. Резерв открытых фондов для увеличения ликвидности (см. п.3)
5. Использование для оплаты комиссий платформы
6. Использование токенов для оплаты товаров и услуг, пример приведен в параграфе 3.2, пример 1.

Приобрести ноус токены изначально можно в момент проведения компанией Pre-ICO, ICO или позже на различных биржах. Для хранения токенов достаточно иметь ERC20 кошелек.

## 7. Вывод
Уже сейчас становится понятно, что блокчейн станет частью нашей жизни, каждый день мы находим все больше подтверждений в прессе, о том, что различные компании успешно реализовали свои пилотные проекты и готовятся к их запуску. Блокчейн обеспечит в ближайшем будущем всем желающим доступ к тем сегментам экономики и промышленности, к которым сейчас имеют доступ только крупные игроки и большие корпорации.

Мы уверены, что ноус протокол станет первым прорывом на пути к открытию свободного инвестирования в любые управляемые токенизированные активы и позволит простым инвесторам стать держателями абсолютно новых видов активов, таких, как солнечная энергия, цифровая недвижимость, майнинговые фермы, игровые артефакты, фьючерсы рынков предсказаний.

Мы также не исключаем, что частные организации или правительства создадут таким образом пенсионные фонды, которые будут прозрачны и понятны для населения.

## Упоминания
[1] BlackRock,Inc https://en.wikipedia.org/wiki/BlackRock
[2] Хедж фонды https://en.wikipedia.org/wiki/List_of_hedge_funds
[3] Инвестиционные банки и компании https://en.wikipedia.org/wiki/List_of_private_equity_firms
[4] Разработчик KYC на блокчейне https://www.civic.com/

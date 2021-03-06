# [usecase - Инвесторы](https://github.com/SerendipityLab/CFSP/blob/master/preWP/rev_2.01_12-28-2017.md#%D0%98%D0%BD%D0%B2%D0%B5%D1%81%D1%82%D0%BE%D1%80%D1%8B-%D1%8D%D0%BA%D1%81%D0%BF%D0%B5%D1%80%D1%82%D1%8B-%D0%BC%D0%B5%D0%BD%D1%82%D0%BE%D1%80%D1%8B-%D0%BF%D1%80%D0%BE%D1%84%D0%B5%D1%81%D1%81%D0%B8%D0%BE%D0%BD%D0%B0%D0%BB%D1%8B)



На основе данных опроса: 

Потребности инвесторов:

- Хотят инвестировать в интересные проекты.
- Хотят тратить время на звездные проекты, в которых есть высокие шансы на успех.
- Не хотят сами заниматься маркетингом и привлекать проекты, не хотят искать проекты, не хотят тратить время на спам проекты.

Проблемы инверсторов:

- Нет никакой информации и возможности понять какой проект выстрелит.
- Практически нет подходов к оценки сырых идей при отсутствии информации.
- Слишком много сырых идей, нет физической возможности собирать информацию о таком количестве людей.
- Нет никакой физической возможности мониторить сотни миллионов сырых идей.

##### Смысл сценария

Инвестор ставит своей целью создание портфеля/ списка людей и проектов, которые по своим показателям показывают лучшие результаты, имеют лучшие прогнозы роста, меньшие риски и необходимый объем данных для принятия решения. Задача инвестора инвестировать деньги или время, и не тратить много времени на анализ и отсев. Для инвестора важно иметь в портфеле проекты с максимальной доходность и при этом высоколиквидны. Предполагается, что выгодные проекты можно держать, а если проект показывает признаки замедления доходности - немедленно слить. Таким образом, смысл данного сценария - формирование списка проектов фаворитов для дальнейшего принятия решения о поддержке.

- На входе сценария у инвестора нет никакой информации, а есть только небольшая сумма, эквивалентная десяткам долларов (может быть любая). 
- На выходе инвестор имеет портфель/список проектов и людей с высшим скором Он может держать и улучшать портфель, а может в любой момент выйти и получить кратную прибыль на вложенный капитал.

Важно, что инвестор взаимодействует не столько с биржей и информацией о проектах, людях, а интерфейсом алгоритма, который формирует портфель в автоматическим режиме, принимая решения или предоставляя это инвестору. Это разные вещи - иметь обоснованную информацию о фаворитах, прогноз их роста, и совершать действия с этой информацией. 


##### Цели сценария 

Создать портфель проинвестированных пректов с лучшими показателями.


##### Сценарий инвестора, желающего сформировать портфель и получать рост его стоимости или доход.

1. Если пользователь хочет поддерживать проект или получить доступ к информациях о проекте и возможностях делать ручной или автоматизированный отбор и скоринг, то он должен купить в на внешней бирже токенов.
2. Покупка происходит по текущему средне взвешенному курсу, учитывающем объем спроса и предложений токена, криптовалют и фиата.
3. Когда пользователь купил токен, он может купить привилегии проектов в ручном режиме, либо с дать задание алгоритму управления портфелем, предварительно настроив его.
4. Если пользователь хочет купить привилегии выбранного проекта, то он выставляет заявку, которая участвует в аукционе, который происходит в реальном времени. Если его предложение отобрано, то происходит сделка, когда он получает привилегии данного проекта, а взмен перечисляет токены. Транзакция происходит автоматически через смарт-контакт, и депонируется в блокчейн.
4. Если пользователь хочет, чтобы формированием портфеля занимался алгоритм, то он производит настроку требований в панели управления алготрейдингом, и запускает процесс. 
6. **Использование алгоритма платное и зависит от объема используемых ресурсов.**
7. Получив задание, алгоритм немедленно начинает формировать портфель, покупая привилегии, соответствующие заданным в настройках критериям. 
8. Купив привилегии, алгоритм получает доступ к скоринговым данным проектов, тем самым получая возможность делать прогнозы и принимать решения о продаже, удержании или покупке новых привилегий прокатов.
9. Алгорит производит ревизию и улучшение портфеля каждый раз, как происходит обновление данных о скорах проектов. Частоту улучшения портфелей можно изменять.
10. Более частое улучшения портфеля тебует больше ресурсов системы, следовательно пользователь больше платит. Если пользователь хочет экономить, то он настраивает меньшую частоту улучшения портфеля, и, таким образом, платит меньше.
11. Алгоритм автоматически на основе анализа решает в каких проектах поддерживать долю, в каких наращивать, а в каких снижать. Если алгоритм нуждается в дополнительных токенах, то он обращается в лимит задепонированных токенов. Если лимит закончился, то алгоритм инициирует запрос инвестору и тот уж принимает решение докупить токенов или взять кредит у системы.
12. Также алгоритм может одолжить токены у системы под определенный процент под залог своего портфел, если инвестор указал такое право. При этом алгоритм может продать часть портфеля, чтобы вернуть долг. Если долг вернуть невозможно, то система автоматически продает часть залога, чтобы вернуть долг.
9. В конечном итоге алгоритм либо наращивает свои позиции, либо продает привилегии прокатов за платежные токены и тем самым фиксирует прибыль.
10. Изменение цены конкретных привилегий и тем самым стоимость портфеля происходит с частотой получения скоринговых данных, которая зависит от частоты ключевых событий в проект и от общего числа проектов в портфеле инвестора. Если в проекте 3 проекта, то очередное изменение скоринга и коррекция цены может происходить раз в неделю. Но если в портфеле тысячи проектов, то изменение цены может происходит несколько раз в секунду. Таким образом, инвестор может очень быстро получать прибыль.
11. Для того, чтобы инвестировать в тысячи проектов - не надо иметь миллионы долларов. Минимальная инвестиция равна 1 токену. Имея 1000 токенов, можно инвестировать в 1000 проектов. Цена токена устанавливается равной 1 доллару и не меняется. Это сделано для того, чтобы токен нельзя было использовать как средство инвестирования, потому что тогда он станет конкурировать с проектами в экосистеме. Поэтому если человек хочет получать прибыль на купленные токены, он должен менять их на привилегии конкретных проектов, которые он уже может продавать. И если привилегии выросли в цене, то инвестор выручает больше токенов, чем заплатил. Таким образом, если он продает токены за фиат, то получает прибыль.

#### Почему качество портфеля улучшается?

- По истечении некоторого минимального периода времени качество портфеля начинает расти, потому что алгоритм динамически управляет составом портфеля, получая скоринговые данные о всех проектах в реальном времени. 
- Математическая модель, лежащая в основе алгоритма приводит к тому, что при большем числе проектов в портфеле и при более длительном периоде анализа, качество портфеля приближается к 100%, что отражается на росте стоимости, потому что стоимость привилегий всех проектов, входящих в портфель неуклонно растет. 
- Почему? Потому что алгоритм способен выбирать правильные проекты на основе своей предиктивной модели.

#### Как работает внутренний рынок? Природа спроса на проекты.

- Поскольку у всех инвесторов в экосистеме такие же алгоритмы, которые отличаются только настройками, то в конечном итоге все инвесторы начинают конкурировать за привилегии проектов-фаворитов. 
- При такой ситуации инвестор если хочет поддерживать объем своей доли в проекте, должен все время поддерживать или наращивать свою долю покупкой новой порции привилегий, конкурируя с остальными участниками рынка. 
- Если он перестает покупать новые привилегии, то его привилегии постепенно размываются вследствие того, что другие инвесторы продолжают бороться за позиции в данном проекте.

#### Математика портфеля

Общий подход описан здесь: 

1. Инновация здесь в том, что человек может входить ничтожными деньгами в огромное число проектов, при этом алгоритм обеспечивает постоянную коррекцию портфеля в сторону увеличения его стоимости.
2. Математика портфеля приводит к тому, что при объеме портфеля не менее 300-400 проектов и при числе итераций скоринга более 100 на промежутке 2-3 недели, в портфеле останутся только те проекты, которые с вероятностью близкой к 100% будут показывать выдающийся рост. 
3. Инвестор может изменять настройки алгоритма так, что в финальном портфеле может оказаться  не более 5% первоначального портфеля, а может не менее 30-40%. Но и остальные проекты не пропадают, потому что алгоритм немедленно продает их на бирже. 
4. Продажа нежелательных проектов может быть с убытком, но прибыль от проектов фаворитов в целом может обеспечивать очень высокую доходность, размер которой зависит только от скорости роста проектов. 
5. Фаворитный портфель, сформированный алгоритмом, может с вероятностью более 80-90% уже не менять существенно свою структуру на длительном промежутке времени. Именно поэтому мы подходим к главное инновации, под названием привилегия.



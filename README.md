Криптография
============

План лекции 19 марта
--------------------

1. Симметричное шифрование: rot13, шифр Цезаря. Шифр подстановки, шифр Виженера, их взлом частотным анализом.
2. Идеальный шифр: одноразовый блокнот. Криптоанализ в случае повторного использования одноразового блокнота.
3. SP-сеть.
3. Арифметика остатков, протокол Диффи-Хеллмана разделение секрета.
Использование Диффи-Хеллмана в качестве асимметричного шифра, шифрованная электронная почта.
5. Коммутативное шифрование: сундук и речка, Pohlig-Hellman. Протокол игры в покер по телефону.


План лекции 26 марта
--------------------

[Слайды с лекции](https://speakerdeck.com/vpavlenko/cryptography-part-2-spring-2014-intellectual-high-school)

1. Режимы блочного шифрования.
2. Хеширование: скорость взлома, fastcoll, length extension attack и HMAC на хэшах.
Процесс джентельменского сообщения о найденной уязвимости.
3. HTTPS: идея шифрования трафика, атака man-in-the-middle, сертификаты и центры сертификации.


План лекции 2 апреля
--------------------

1. Trusted timestamping.
1. Биткоины.
2. Обсуждение домашней работы. Будет рассказано решение номеров 2-3 (их больше нельзя будет зачесть).


Ссылки
------

1. Википедия:
[ROT13](http://ru.wikipedia.org/wiki/ROT13),
[одноразовый блокнот](http://ru.wikipedia.org/wiki/%D0%9D%D0%B5%D0%B2%D0%B7%D0%BB%D0%B0%D0%BC%D1%8B%D0%B2%D0%B0%D0%B5%D0%BC%D1%8B%D0%B9_%D1%88%D0%B8%D1%84%D1%80),
[симметричный шифр DES](http://ru.wikipedia.org/wiki/DES).
[Малая теорема Ферма](http://ru.wikipedia.org/wiki/%D0%9C%D0%B0%D0%BB%D0%B0%D1%8F_%D1%82%D0%B5%D0%BE%D1%80%D0%B5%D0%BC%D0%B0_%D0%A4%D0%B5%D1%80%D0%BC%D0%B0),
[протокол Диффи-Хеллмана](http://ru.wikipedia.org/wiki/%D0%9F%D1%80%D0%BE%D1%82%D0%BE%D0%BA%D0%BE%D0%BB_%D0%94%D0%B8%D1%84%D1%84%D0%B8_%E2%80%94_%D0%A5%D0%B5%D0%BB%D0%BB%D0%BC%D0%B0%D0%BD%D0%B0),
[RSA](http://ru.wikipedia.org/wiki/RSA),
[SSH](http://ru.wikipedia.org/wiki/SSH),
[SSL](http://ru.wikipedia.org/wiki/SSL).

2. [План семестрового курса по криптографии](https://www.cs.purdue.edu/homes/ninghui/courses/555_Spring12/lectures.html)
в случайно выбранном западном университете

3. [Обсуждение покера по телефону на русском языке](http://logic.pdmi.ras.ru/~yura/crypto/02byzant.pdf)

4. [Уязвимость во Flickr'e - length-extension attack на MD5](http://netifera.com/research/flickr_api_signature_forgery.pdf)

5. [Основная статья про биткоины](https://bitcoin.org/bitcoin.pdf)


Задания
-------

Все задания сдаются письменно, ответы и флаги отправляются на электронную почту vpavlenko.int@gmail.com
вместе с подробным описанием того, как эти ответы и флаги были добыты.
Прошу извещать меня сразу же, как только вам удастся решить хотя бы одну задачу. Это позволит мне мониторить
вашу активность.

Обязательная часть: 45 баллов. Для получения пятёрки за задание надо получить хотя бы 35 баллов.

1. (5 баллов)
Гриша был зарегистрирован на одном сайте, базу паролей которого недавно взломали и выложили. Хэш его пароля: 3517c55f3ffdd3322ccbe12039e33758. Сколько ему лет?

2. (10 баллов)
[Электронный журнал на асимметричном шифровании](marks/)

3. (10 баллов)
Можно ли в качестве коммутативного шифра при игре в покер использовать XOR (одноразовый блокнот)?

4. (10 баллов)
[Передайте сообщение, используя асимметричное шифрование](public-key/)

5. (10 баллов)
Предлагаю вам обыграть меня в покер по переписке. Тасуйте колоду. Присылайте
колоду и инструкции мне на почту, я сдам себе и вам пять карт.

4. (15 баллов)
[Это духовой инструмент или струнный?](sub.txt) Впрочем, меня интересует сам флаг

6. (15 баллов)
Похоже, файл dest.jpg в папке [jpeg](jpeg) зашифрован. Может, в нём был записан флаг?

7. (15 баллов)
А может ли флаг быть спрятан в самом ключе? См. папку [vigenere](vigenere)

8. (15 баллов)
Задача взята с http://ufologists.ictis.sfedu.ru/:

        Моя веселая ФЕРМА
        
        Играя в свою любимую игру, я наткнулся на данные ниже. Помогите разобраться с этим! Я хочу купить новый хвост для коровы.
        {"n":55730048063717018374316281207573259125944928596988375563008761242928555444475159973323697033529485947694144334157841984089222608221659443869403243311377775287940043976050079897679344195429140671152006335092107296007295641129810127120597697958505609557108821553087048650668127879505133240481364133955404508724801433652620134539765901833015644832323224073360418288546329260222548709056388931692867087156683666545959017505300012887342748040633895056662119255382438961050252741419077501234468618586586761527436899702065013210399451488547753808782146177428317609036251342347553017178247158741715583011215815698806579497027,
        "e":65537,
        "enc_data":25234514147851501650928728210405740434891970671488428405196440434538180451319426356822060051035053769070087646943825115802785624107829588035763512660763770355863470442359006751937231446693677756587159506517057107545904847781133985450962418304405156723626987851757046221296000186129919558271304842917074255645894198513219579694940888303668954853572211412406774298397963087228995608199961416160365961933944487096937024121738220372895375686782970385612792024930159117151472088279156003279742341584430863692287750584160827079689586790181031407137862737274577936446435723045268025310178271959285118689249074803904304795181}

8. (15 баллов)
Задача взята с http://ufologists.ictis.sfedu.ru/:

        Самый надежный шифр - это одноразовый блокнот, но мне лень придумывать много... 
        
        2426d6c3ef1a29652be80311a82c031d3ba564992d2fbf1d3bb3bee6cb523187e64ecb1af636b0a492571de1ac693ca10483736ee37912ccf544233c5507f14a14a8da2877a2b0d16a8cb90ce91bc0192fe733b4b254e834b943bf41278cf922314c9f8433 
        242193b0cf1d236520ff145ce339140b69ec65dc2c2fbe0f77abf0f08e502885e759db1af62bf1bc834154f0e97b3ae445897d71f965128df456232e5210f15615be8e3460b8e5cc65d8a35eff0d94153aec22b0b54aba20b90ba24d2796f4226559879571 
        2921c6c3c11c2a683dba081fb769050672a27c992e2eba0c77b3f1e18e563f80ee4f8f4af836e3b9985e44a3a8743bf600923075fe721589ba53762d4e16b84d13a88e306caff89e7fc3fa12f91fc01a2db537bcaa42bb34bb06eb5a68c5f939741c87872b 
        2726d68d8c0c227569f60311b127510f3ba076d73d33ba1f32e6bef8c7462490ec42c15dbb65e3a09f5356eaa77d68e00b843076e47e1285f44523294f07f14b10abc13571bafeca208cb80be44bc61329f13baabd0dab20a743aa42748aad33741c9c832d 
        316ec08ac105216569ee0308b769170777a937d73f23bf0b77a4f1b4cf51349cf642c054f629b0bd9f465ce7a86e29a1118f3060e5640f9fee0277205842a3471cbfcb3525b2fe9e65c2ae1be21bc6133cf426adb543e461a80daf0e738de823745a85943a 
        2426d6c3ca07286569ec0302b0201e0035ec5ecd7a25b41623abf7fadd1531d5e144c257f62bf4f0965b53e6e97326f500927660f5724accfc4e622f4610e2161184cd357cabe48e53eeb330f75beb2e07c72fe4bf5da42ea017aa5a6e8ae37170528ec632 
        3c2fc786de553a693df24604ab2c510d74a076c92923fb1731eacce1dd463994ec0bea57e72ce2b5da4655e6e96f26e813856272ff631fcced4370685303bc4719fbea286ba8fbd1758c8f10f91dd1043bfc26bdfa4cae35ac11deb5a6f80ad23745b838931

# League of Legends рейтинг ойындарына талдау

__League of Legends__ - бес чемпионнан (ойын ішіндегі кейіпкерлер атауы) тұратын екі команда жау базасын жою үшін бір-бірімен соғысатын стратегиялық бірлескен MOBA жанрындағы ойын. 

Ойынның басты мақсаты: өзге команданың нексусын жою. 

Сіздің нексус - миниондар пайда болатын жер. Нексустың артында денсаулық пен мананы тез қалпына келтіруге, сондай-ақ дүкеннен заттарды сатып алуға болатын субұрқақ бар.

![image](https://github.com/Nuray-web/lol_analysis/assets/72253666/4f4210ed-14d4-43db-a28b-373d8ab89f8d)

Қарсылас нексусқа жету үшін сіздің командаңыз кем дегенде бір жолақты босатуы керек. Бірақ мұны істеу оңай емес, өйткені жолды қорғаныс құрылымдары - мұнаралар мен ингибиторлар жауып тастайды. Әрбір жолдың үш мұнарасы және бір ингибиторы бар, ал нексус тағы екі мұнарамен қорғалады.

Жолақтар арасында бейтарап құбыжықтар өмір сүретін және өсімдіктер гүлдейтін орман бар. Ойынның ең маңызды құбыжықтары - барон Нашор және айдаһарлар. Бұл жауынгерлерді өлтіру сіздің командаңызға ойынның ағымын өзгерте алатын бірегей басымдылықтарды береді.

[Қалай ойнау керек?](https://www.leagueoflegends.com/ru-ru/how-to-play/)

Ойынның нәтижесін матчтың алғашқы 10 минутында анықтауға болатынын не болмайтынын білу үшін рейтингі жоғары (Diamond-Master)   матчтардың деректерін қарастырамыз.

[Деректерге қол жеткізу.](https://www.kaggle.com/datasets/bobbyscience/league-of-legends-diamond-ranked-games-10-min)

Датасет туралы айта кететін болсақ, әр топқа 20 ерекше параметрлерден келеді.

Анализ бастамай тұрып, сізге білу керек деректер бойынша глоссарий:

- Warding totem (Vision, қысқаша тотем немесе вард) - Ойыншы картада жақын маңдағы аумақты көруге мүмкіншілік алу үшін қоя алатын зат. Карта я болмаса құбыжықтарды бақылау мақсатында өте пайдалы.
- Minions (миниондар, криптер, фарм) - екі командаға тиесілі NPC. Ойыншылар оларды өлтірген кезде алтын алады.
- Jungle minions (қысқаша жай ғана орман) - ешбір топқа жатпайтын NPC. Ойыншылар оларды өлтірген кезде алтын мен қосымша пайдалы эффекттер (бафф) алады.
- Elite Monsters (ерекше құбыжықтар): команда өлтірген кезде үлкен бонус (алтын/XP(тәжірибе)/стат(кейіпкер параметрлеріне қосымша)) беретін зор денсаулығы/зақымы бар құбыжықтар.
- Dragons (айдаһарлар): өлтірілген кезде командаға бонус беретін және карта ландшафтын өзгертетін ерекше құбыжық. Белгілі бір команда өлтірген 4-ші айдаһар түріне байланысты статистикалық бонус береді. 5-ші айдаһар (аға айдаһар) командаға зор артықшылық береді.
- Herald (Геральд): Ойыншы өлтірген кезде статистикалық бонус беретін ерекше құбыжық. Бұл жолақта жауға қысым көрсетуге көмектеседі және құрылымдарды бұзады.

Қарастырылған деректер бойынша, кейіпкерлер мен олардың жинаған артефакттары саналмайды, бірақ олардың ойынға ықпалы жоқ болғанынан емес - ақпараттың толық болмағанынан. Бұл талдауда біз жалпы макро-ойын туралы және жалпы ойын барысында ойыншы неге назар аудару керегін көреміз.

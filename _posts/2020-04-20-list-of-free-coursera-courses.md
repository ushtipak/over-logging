---
title: "List of free Coursera courses"
categories: [coursera, selenium]
---


Coursera is by far the most advanced learning platform

Only downside is that most courses are now pay-as-you-go, with honorable exceptions

![Pepperidge Farm Remembers]({{ site.url }}{{ site.baseurl}}/assets/2020-04-20-list-of-free-coursera-courses/pepperidge-farm-remembers.jpg)
> src: [Imgflip](https://imgflip.com/memegenerator/)


Primarily IT ones are pay-only, with some that allow audit,
but that is rarely sufficient, since the exercises, peer reviews
and labs are not included

Thankfully there are plenty that are still free; excluding a certificate, of course

Which ones, however, can't be easily distinguished, aside from logging in
and selecting "Enroll" to see the actual options


# WebDriver delight

To create list of the kind, programmatically, Selenium, with Mozilla's GeckoDriver, was used

It allowed a `as-human-as-possible` data retrieval in three phases:

* Get [all categories](https://github.com/ushtipak/coursera-scout/blob/master/stage_1_get_categories.py) (parsing retrieved apollo-client state)
* Retrieve [surface info](https://github.com/ushtipak/coursera-scout/blob/master/stage_2_get_courses.py) on all courses from all categories
* Check [enrollment options](https://github.com/ushtipak/coursera-scout/blob/master/stage_3_get_offerings.py) for each (with login and simulated activity)

Same setup yielded an additional list of courses that are [available for audit](http://localhost:4000/over-logging/coursera/selenium/2020/04/21/auditable-coursera-courses.html)


# Categories

![Coursera]({{ site.url }}{{ site.baseurl}}/assets/2020-04-20-list-of-free-coursera-courses/coursera.png)


Jump to preferred category or scroll through all 1485 courses:

* [arts-and-humanities/history](#arts-and-humanitieshistory)
* [arts-and-humanities/music-and-art](#arts-and-humanitiesmusic-and-art)
* [arts-and-humanities/philosophy](#arts-and-humanitiesphilosophy)
* [business/business-essentials](#businessbusiness-essentials)
* [business/business-strategy](#businessbusiness-strategy)
* [business/entrepreneurship](#businessentrepreneurship)
* [business/finance](#businessfinance)
* [business/leadership-and-management](#businessleadership-and-management)
* [business/marketing](#businessmarketing)
* [computer-science/algorithms](#computer-sciencealgorithms)
* [computer-science/computer-security-and-networks](#computer-sciencecomputer-security-and-networks)
* [computer-science/design-and-product](#computer-sciencedesign-and-product)
* [computer-science/mobile-and-web-development](#computer-sciencemobile-and-web-development)
* [computer-science/software-development](#computer-sciencesoftware-development)
* [data-science/data-analysis](#data-sciencedata-analysis)
* [data-science/machine-learning](#data-sciencemachine-learning)
* [data-science/probability-and-statistics](#data-scienceprobability-and-statistics)
* [information-technology/cloud-computing](#information-technologycloud-computing)
* [information-technology/data-management](#information-technologydata-management)
* [information-technology/networking](#information-technologynetworking)
* [information-technology/security](#information-technologysecurity)
* [language-learning/learning-english](#language-learninglearning-english)
* [language-learning/other-languages](#language-learningother-languages)
* [life-sciences/animal-health](#life-sciencesanimal-health)
* [life-sciences/basic-science](#life-sciencesbasic-science)
* [life-sciences/healthcare-management](#life-scienceshealthcare-management)
* [life-sciences/health-informatics](#life-scienceshealth-informatics)
* [life-sciences/nutrition](#life-sciencesnutrition)
* [life-sciences/patient-care](#life-sciencespatient-care)
* [life-sciences/psychology](#life-sciencespsychology)
* [life-sciences/public-health](#life-sciencespublic-health)
* [life-sciences/research](#life-sciencesresearch)
* [math-and-logic/math-and-logic](#math-and-logicmath-and-logic)
* [personal-development/personal-development](#personal-developmentpersonal-development)
* [physical-science-and-engineering/chemistry](#physical-science-and-engineeringchemistry)
* [physical-science-and-engineering/electrical-engineering](#physical-science-and-engineeringelectrical-engineering)
* [physical-science-and-engineering/environmental-science-and-sustainability](#physical-science-and-engineeringenvironmental-science-and-sustainability)
* [physical-science-and-engineering/mechanical-engineering](#physical-science-and-engineeringmechanical-engineering)
* [physical-science-and-engineering/physics-and-astronomy](#physical-science-and-engineeringphysics-and-astronomy)
* [physical-science-and-engineering/research-methods](#physical-science-and-engineeringresearch-methods)
* [social-sciences/economics](#social-scienceseconomics)
* [social-sciences/education](#social-scienceseducation)
* [social-sciences/governance-and-society](#social-sciencesgovernance-and-society)
* [social-sciences/law](#social-scienceslaw)


# Courses by category

## arts-and-humanities/history

* [Roman Architecture](https://www.coursera.org/learn/roman-architecture) Yale University
* [Indigenous Canada](https://www.coursera.org/learn/indigenous-canada) University of Alberta
* [Egiptología (Egyptology)](https://www.coursera.org/learn/egypt) Universitat Autònoma de Barcelona
* [Age of Cathedrals](https://www.coursera.org/learn/age-of-cathedrals) Yale University
* [Feminism and Social Justice](https://www.coursera.org/learn/feminism-social-justice) University of California, Santa Cruz
* [A Journey through Western Christianity: from Persecuted Faith to Global Religion (200 - 1650)](https://www.coursera.org/learn/western-christianity-200-1650) Yale University
* [The Ancient Greeks](https://www.coursera.org/learn/ancient-greeks) Wesleyan University
* [The Holocaust - An Introduction (I): Nazi Germany: Ideology, The Jews and the World](https://www.coursera.org/learn/holocaust-introduction-1) Tel Aviv University
* [Russian History: from Lenin to Putin](https://www.coursera.org/learn/russian-history-lenin-putin) University of California, Santa Cruz
* [The Emergence of the Modern Middle East - Part I](https://www.coursera.org/learn/modern-middle-east-1) Tel Aviv University
* [Film, Images & Historical Interpretation in the 20th Century: The Camera Never Lies](https://www.coursera.org/learn/film-images) University of London
* [Iniciación a los jeroglíficos egipcios](https://www.coursera.org/learn/iniciacion-jeroglificos-egipcios) Universitat Autònoma de Barcelona
* [The History of Modern Israel – Part I: From an Idea to a State](https://www.coursera.org/learn/history-israel) Tel Aviv University
* [American Education Reform: History, Policy, Practice](https://www.coursera.org/learn/edref) University of Pennsylvania
* [The Fall and Rise of Jerusalem](https://www.coursera.org/learn/jerusalem) Tel Aviv University
* [История и теория медиа (History and theory of media)](https://www.coursera.org/learn/teoriya-smi) National Research University Higher School of Economics
* [At the Origins of the Mediterranean Civilization: Archaeology of the City from the Levant to the West - 3rd-1st millennium BC](https://www.coursera.org/learn/archaeology-city-levant-west) Sapienza University of Rome
* [El Valle de los Reyes](https://www.coursera.org/learn/valle-de-los-reyes) Universitat Autònoma de Barcelona
* [A Voice of Their Own. Women's Spirituality in the Middle Ages.](https://www.coursera.org/learn/womens-spirituality) Universitat de Barcelona
* [Introduction to Who Wrote Shakespeare](https://www.coursera.org/learn/shakespeare) University of London
* [Stalin and Stalinism in Russian History](https://www.coursera.org/learn/stalinism) National Research University Higher School of Economics
* [The Changing Landscape of Ancient Rome. Archaeology and History of the Palatine Hill](https://www.coursera.org/learn/palatine-hill-archaeology-history) Sapienza University of Rome
* [The Talmud: A Methodological Introduction](https://www.coursera.org/learn/the-talmud) Northwestern University
* [史記 (Shi Ji)](https://www.coursera.org/learn/shiji) National Taiwan University
* [The Holocaust - An Introduction (II): The Final Solution](https://www.coursera.org/learn/holocaust-introduction-2) Tel Aviv University
* [中國古代歷史與人物：秦始皇（Qin Shi Huang)](https://www.coursera.org/learn/qin-shi-huang) National Taiwan University
* [The Emergence of the Modern Middle East - Part II](https://www.coursera.org/learn/modern-middle-east-2) Tel Aviv University
* [Art of the MOOC: Experiments with Sound](https://www.coursera.org/learn/experiments-with-sound) Duke University
* [A Brief History of Human Spaceflight](https://www.coursera.org/learn/human-spaceflight) University of Houston System
* [The Holocaust: The Destruction of European Jewry](https://www.coursera.org/learn/the-holocaust) University of California, Santa Cruz
* [Exploring Beethoven’s Piano Sonatas Part 2](https://www.coursera.org/learn/exploring-beethoven-piano-sonatas-2) Curtis Institute of Music
* [Paesaggi di Roma Antica. Archeologia e storia del Palatino.](https://www.coursera.org/learn/paesaggi-roma-antica) Sapienza University of Rome
* [Intellectual Change in Early China: Warring States and Han](https://www.coursera.org/learn/intellectual-change-early-china-the-warring-states-han) The Chinese University of Hong Kong
* [Calvin - Histoire et réception d'une Réforme](https://www.coursera.org/learn/calvin) University of Geneva
* [The History of Modern Israel - Part II: Challenges of Israel as a sovereign state](https://www.coursera.org/learn/history-israel-sovereign-state) Tel Aviv University
* [Arch of Titus: Rome and the Menorah](https://www.coursera.org/learn/archoftitus) Yeshiva University
* [現代文學導讀：詩、散文、小說](https://www.coursera.org/learn/poetry-prose-novel) National Taiwan University
* [Religious Transformation in Early China: the Period of Division](https://www.coursera.org/learn/religious-transformation-early-china-the-period-of-division) The Chinese University of Hong Kong
* [Alle origini della civiltà mediterranea: archeologia della città dal Levante all’Occidente - III-I millennio a.C.](https://www.coursera.org/learn/nigro-levante-occidente) Sapienza University of Rome
* [Диаспоры в глобальной политике](https://www.coursera.org/learn/diaspori-v-globalnoi-politike) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Exploring Beethoven's Piano Sonatas Part 5](https://www.coursera.org/learn/exploring-beethoven-piano-sonatas-5) Curtis Institute of Music
* [Structuring Values in Modern China](https://www.coursera.org/learn/structuring-values-modern-china) The Chinese University of Hong Kong
* [Religion and Thought in Modern China: the Song, Jin, and Yuan](https://www.coursera.org/learn/religion-thought-modern-china) The Chinese University of Hong Kong
* [Exploring Beethoven's Piano Sonatas Part 6](https://www.coursera.org/learn/exploring-beethoven-piano-sonatas-6) Curtis Institute of Music
* [Exploring Beethoven's Piano Sonatas Part 4](https://www.coursera.org/learn/exploring-beethoven-piano-sonatas-4) Curtis Institute of Music
* [中日文化交流史](https://www.coursera.org/learn/zhongri-jiaoliushi) Peking University
* [生命科学发展史](https://www.coursera.org/learn/shengming-kexue-fazhanshi) Shanghai Jiao Tong University
* [Thomas Berry的世界观：地球社区的繁荣 (The Worldview of Thomas Berry: The Flourishing of the Earth Community)](https://www.coursera.org/learn/diqiu-fanrong) Yale University


## arts-and-humanities/music-and-art

* [Modern Art & Ideas](https://www.coursera.org/learn/modern-art-ideas) The Museum of Modern Art
* [Seeing Through Photographs](https://www.coursera.org/learn/photography) The Museum of Modern Art
* [Fashion as Design](https://www.coursera.org/learn/fashion-design) The Museum of Modern Art
* [Introduction to Classical Music](https://www.coursera.org/learn/introclassicalmusic) Yale University
* [Guitar for Beginners](https://www.coursera.org/learn/guitar) Berklee College of Music
* [In the Studio: Postwar Abstract Painting](https://www.coursera.org/learn/painting) The Museum of Modern Art
* [Write Your First Novel](https://www.coursera.org/learn/write-your-first-novel) Michigan State University
* [Guitar Scales and Chord Progressions](https://www.coursera.org/learn/guitar-scales-chord-progressions) Berklee College of Music
* [Art & Activity: Interactive Strategies for Engaging with Art](https://www.coursera.org/learn/art-activity) The Museum of Modern Art
* [Modern & Contemporary American Poetry (“ModPo”)](https://www.coursera.org/learn/modpo) University of Pennsylvania
* [Art & Ideas: Teaching with Themes](https://www.coursera.org/learn/ideas) The Museum of Modern Art
* [Sharpened Visions: A Poetry Workshop](https://www.coursera.org/learn/poetry-workshop) California Institute of the Arts
* [Introducción a la guitarra](https://www.coursera.org/learn/guitarra) Berklee College of Music
* [Script Writing: Write a Pilot Episode for a TV or Web Series (Project-Centered Course)](https://www.coursera.org/learn/script-writing) Michigan State University
* [Jazz Improvisation](https://www.coursera.org/learn/jazz-improvisation) Berklee College of Music
* [The Language of Design: Form and Meaning](https://www.coursera.org/learn/design-language) California Institute of the Arts
* [Write A Feature Length Screenplay For Film Or Television](https://www.coursera.org/learn/write-a-feature-length-screenplay-for-film-or-television) Michigan State University
* [The Music of the Beatles](https://www.coursera.org/learn/the-beatles) University of Rochester
* [Approaching Music Theory: Melodic Forms and Simple Harmony](https://www.coursera.org/learn/melodic-forms-simple-harmony) California Institute of the Arts
* [History of Rock, Part One](https://www.coursera.org/learn/history-of-rock) University of Rochester
* [Leer a Macondo: la obra de Gabriel García Márquez](https://www.coursera.org/learn/macondo-gabriel-garcia-marquez) Universidad de los Andes
* [ART of the MOOC: Public Art and Pedagogy](https://www.coursera.org/learn/public-art-pedagogy) Duke University
* [Fundamentals of Audio and Music Engineering: Part 1 Musical Sound & Electronics](https://www.coursera.org/learn/audio-engineering) University of Rochester
* [Exploring Beethoven’s Piano Sonatas](https://www.coursera.org/learn/beethoven-piano-sonatas) Curtis Institute of Music
* [Producción Musical y su Efecto en la Composición](https://www.coursera.org/learn/produccionycomposicion) Berklee College of Music
* [Music as Biology: What We Like to Hear and Why](https://www.coursera.org/learn/music-as-biology) Duke University
* [VR and 360 Video Production](https://www.coursera.org/learn/360-vr-video-production) Google AR & VR
* [Improvisación de jazz](https://www.coursera.org/learn/improvisacion-de-jazz) Berklee College of Music
* [Write Like Mozart: An Introduction to Classical Music Composition](https://www.coursera.org/learn/classical-composition) National University of Singapore
* [The Blues: Understanding and Performing an American Art Form](https://www.coursera.org/learn/the-blues) University of Rochester
* [Sexing the Canvas: Art and Gender](https://www.coursera.org/learn/gender-art) The University of Melbourne
* [Arranging for Songwriters](https://www.coursera.org/learn/arranging-for-songwriters) Berklee College of Music
* [The Cycle: Management of Successful Arts and Cultural Organizations](https://www.coursera.org/learn/the-cycle) University of Maryland, College Park
* [Words Spun Out of Images: Visual and Literary Culture in Nineteenth Century Japan](https://www.coursera.org/learn/visual-literary-culture-in-japan) The University of Tokyo
* [Introducción al Arte Sonoro](https://www.coursera.org/learn/introduccion-arte-sonoro) Universitat de Barcelona
* [唐詩新思路 (Tang Poetry)](https://www.coursera.org/learn/tang-poems) National Taiwan University
* [Teaching the Violin and Viola: Creating a Healthy Foundation](https://www.coursera.org/learn/teach-violin-lessons) Northwestern University
* [ART of the MOOC: Activism and Social Movements](https://www.coursera.org/learn/activism-social-movements) Duke University
* [Scandinavian Film and Television](https://www.coursera.org/learn/scandinavian-movies-tv) University of Copenhagen
* [Deciphering Secrets: The Illuminated Manuscripts of Medieval Europe](https://www.coursera.org/learn/medieval-europe) University of Colorado System
* [Teoria Musical](https://www.coursera.org/learn/teoria-musical) Berklee College of Music
* [Introduzione alla Storia dell'Architettura Contemporanea](https://www.coursera.org/learn/architettura-contemporanea) Politecnico di Milano
* [Entreprendre dans les Industries Culturelles à l'ère du numérique](https://www.coursera.org/learn/entreprendre-culture) Sciences Po
* [Theatre and Globalization](https://www.coursera.org/learn/global-theatre) Ludwig-Maximilians-Universität München (LMU)
* [The World of the String Quartet](https://www.coursera.org/learn/string-quartet) Curtis Institute of Music
* [Fundamentals of Rehearsing Music Ensembles](https://www.coursera.org/learn/music-ensembles) The University of North Carolina at Chapel Hill
* [Asian Environmental Humanities: Landscapes in Transition](https://www.coursera.org/learn/asian-environmental-humanities) University of Zurich
* [The Mediterranean, a Space of Exchange (from the Renaissance to Enlightenment)](https://www.coursera.org/learn/mediterraneanhistory) Universitat de Barcelona
* [Copyright for Multimedia](https://www.coursera.org/learn/copyright-for-multimedia) Duke University
* [Today’s Music Industry](https://www.coursera.org/learn/music-industry) West Virginia University
* [History of Rock, Part Two](https://www.coursera.org/learn/history-of-rock-2) University of Rochester
* [Online Games: Literature, New Media, and Narrative](https://www.coursera.org/learn/interactive-media-gaming) Vanderbilt University
* [Leading Innovation in Arts and Culture](https://www.coursera.org/learn/arts-culture-innovation) Vanderbilt University
* [A complexidade sensível: Um paralelo entre videogames e arte](https://www.coursera.org/learn/videogames) Universidade Estadual de Campinas
* [Recovering the Humankind's Past and Saving the Universal Heritage](https://www.coursera.org/learn/preserving-cultural-heritage) Sapienza University of Rome
* [Classics of Chinese Humanities: Guided Readings](https://www.coursera.org/learn/classics-chinese-humanities) The Chinese University of Hong Kong
* [So You Think You Know Tango?](https://www.coursera.org/learn/tango) Emory University
* [ART of the MOOC: Arte Público y Pedagogía](https://www.coursera.org/learn/arte-publico-pedagogia) Duke University
* [Modern Hebrew Poetry שירה עברית מודרנית](https://www.coursera.org/learn/hebrew-poetry) Hebrew University of Jerusalem
* [Introdução à Guitarra](https://www.coursera.org/learn/intro-guitarra) Berklee College of Music
* [透过摄影看世界](https://www.coursera.org/learn/sheying) The Museum of Modern Art
* [ART of the MOOC: Activismo y Movimientos Sociales](https://www.coursera.org/learn/activismo-movimientos-sociales) Duke University
* [東坡詞 (Ci Poetry of Su Dong Po)](https://www.coursera.org/learn/su-dongpo) National Taiwan University
* [崑曲之美](https://www.coursera.org/learn/kunqu) The Chinese University of Hong Kong
* [Music's Big Bang: The Genesis of Rock 'n' Roll](https://www.coursera.org/learn/rock-and-roll-music) University of Florida
* [The Music of the Rolling Stones, 1962-1974](https://www.coursera.org/learn/rolling-stones) University of Rochester
* [Exploring Beethoven's Piano Sonatas Part 3](https://www.coursera.org/learn/exploring-beethoven-piano-sonatas-3) Curtis Institute of Music
* [Be entrepreneurial in Cultural Industries in the digital age](https://www.coursera.org/learn/entrepreneurial-culture-digital-age) Sciences Po
* [The Beauty of Kunqu Opera](https://www.coursera.org/learn/kunqu-opera) The Chinese University of Hong Kong
* [中國人文經典導讀](https://www.coursera.org/learn/zhongguorenwenjingdiandaodu) The Chinese University of Hong Kong
* [20世纪西方音乐 Western Music in the 20th Century](https://www.coursera.org/learn/20cnwm) Peking University
* [Improvisação no Jazz](https://www.coursera.org/learn/improvisacao-no-jazz) Berklee College of Music
* [Science and Technology in the Silla Cultural Heritage](https://www.coursera.org/learn/silla-science-technology) Pohang University of Science and Technology


## arts-and-humanities/philosophy

* [Introduction to Philosophy](https://www.coursera.org/learn/philosophy) The University of Edinburgh
* [Moral Foundations of Politics](https://www.coursera.org/learn/moral-politics) Yale University
* [Ancient Philosophy: Plato & His Predecessors](https://www.coursera.org/learn/plato) University of Pennsylvania
* [Social Norms, Social Change I](https://www.coursera.org/learn/norms) University of Pennsylvania
* [Pensamiento Científico](https://www.coursera.org/learn/ciencia) Universidad Nacional Autónoma de México
* [Effective Altruism](https://www.coursera.org/learn/altruism) Princeton University
* [Основы философии: о чем спорят философы сегодня](https://www.coursera.org/learn/osnovy-filosofii) National Research University Higher School of Economics
* [The Modern and the Postmodern (Part 1)](https://www.coursera.org/learn/modern-postmodern-1) Wesleyan University
* [Emotions: a Philosophical Introduction](https://www.coursera.org/learn/emotions) Universitat Autònoma de Barcelona
* [Music and Social Action](https://www.coursera.org/learn/music-and-social-action) Yale University
* [Gabriel García Márquez entre el poder, la historia y el amor](https://www.coursera.org/learn/gabriel-garcia-marquez-poder-historia-amor) Universidad de los Andes
* [Ancient Philosophy: Aristotle and His Successors](https://www.coursera.org/learn/aristotle) University of Pennsylvania
* [Philosophy and the Sciences: Introduction to the Philosophy of Cognitive Sciences](https://www.coursera.org/learn/philosophy-cognitive-sciences) The University of Edinburgh
* [Søren Kierkegaard - Subjectivity, Irony and the Crisis of Modernity](https://www.coursera.org/learn/kierkegaard) University of Copenhagen
* [Humanidades digitales](https://www.coursera.org/learn/humanidades-digitales) Universitat Autònoma de Barcelona
* [Philosophy, Science and Religion: Science and Philosophy](https://www.coursera.org/learn/philosophy-science-religion-1) The University of Edinburgh
* [Philosophy and the Sciences: Introduction to the Philosophy of Physical Sciences](https://www.coursera.org/learn/philosophy-physical-sciences) The University of Edinburgh
* [Philosophy, Science and Religion: Philosophy and Religion](https://www.coursera.org/learn/philosophy-science-religion-2) The University of Edinburgh
* [Love as a Force for Social Justice](https://www.coursera.org/learn/love-social-justice) Stanford University
* [Revolutionary Ideas: Utility, Justice, Equality, Freedom](https://www.coursera.org/learn/revolutionary-ideas-utility-justice-equality-freedom) Rutgers the State University of New Jersey
* [Философия культуры (Philosophy of Culture)](https://www.coursera.org/learn/filosofiya-kultury) National Research University Higher School of Economics
* [Organising an Empire: The Assyrian Way](https://www.coursera.org/learn/organising-empire-assyrian-way) Ludwig-Maximilians-Universität München (LMU)
* [Social Norms, Social Change II](https://www.coursera.org/learn/change) University of Pennsylvania
* [The Modern and the Postmodern (Part 2)](https://www.coursera.org/learn/modern-postmodern-2) Wesleyan University
* [Violences et religions](https://www.coursera.org/learn/violences-religions) University of Geneva
* [Reason and Persuasion: Thinking Through Three Dialogues By Plato](https://www.coursera.org/learn/plato-dialogues) National University of Singapore
* [Designing the Future of Work](https://www.coursera.org/learn/designing-future-of-work) UNSW Sydney (The University of New South Wales)
* [莊子─姿勢、意識與感情 (Zhuangzi─Posture, Awareness, and Sentiment)](https://www.coursera.org/learn/zhuangzi) National Taiwan University
* [Philosophy, Science and Religion: Religion and Science](https://www.coursera.org/learn/philosophy-science-religion-3) The University of Edinburgh
* [The Importance and Power of Music in our Society](https://www.coursera.org/learn/importance-power-music-our-society) Universiteit Leiden
* [Moses' Face: Moses' images as reflected in Jewish literature](https://www.coursera.org/learn/moses) Hebrew University of Jerusalem
* [Inequality and Democracy](https://www.coursera.org/learn/inequality-and-democracy) Utrecht University
* [Science & Religion 101](https://www.coursera.org/learn/science-and-religion-101) University of Alberta
* [Revolutionary Ideas: Borders, Elections, Constitutions, Prisons](https://www.coursera.org/learn/revolutionary-ideas-borders-elections-constitutions-prisons) Rutgers the State University of New Jersey
* [活用希臘哲學 (Understanding the Greek Philosophy)](https://www.coursera.org/learn/xila-zhexue) National Taiwan University
* [莊子─人情 (Zhuangzi─Between People)](https://www.coursera.org/learn/zhuangzi2) National Taiwan University
* [東亞儒家：人文精神一(East Asian Confucianisms: Humanism (1))](https://www.coursera.org/learn/east-asian-confucianisms-humanism1) National Taiwan University
* [Luther and the West](https://www.coursera.org/learn/luther-and-the-west) Northwestern University
* [哲学导论（中文版）](https://www.coursera.org/learn/zhexue-daolun) The University of Edinburgh
* [Relativism](https://www.coursera.org/learn/relativism) University of California, Irvine
* [Ecologie Politique: défi de la durabilité pour les démocraties](https://www.coursera.org/learn/ecologie-politique) University of Lausanne
* [When Disaster Meets Conflict](https://www.coursera.org/learn/whendisastermeetsconflict) Erasmus University Rotterdam
* [The Politics of Skepticism](https://www.coursera.org/learn/erasmus-philosophy-skepticism) Erasmus University Rotterdam
* [紅樓夢(The Red Chamber Dream)](https://www.coursera.org/learn/the-red-chamber-dream) National Taiwan University
* [中国哲学经典著作导读](https://www.coursera.org/learn/chinese-philosophy) Xi'an Jiaotong University
* [On Being a Scientist](https://www.coursera.org/learn/scientist) Universiteit Leiden
* [Soul Beliefs: Causes and Consequences - Unit 2: Belief Systems](https://www.coursera.org/learn/soulbeliefs2) Rutgers the State University of New Jersey
* [Мой друг - робот: введение в социальную робототехнику / My Friend is a Robot: Introduction to Social Robotics](https://www.coursera.org/learn/moy-drug-robot) National Research Tomsk State University
* [東亞儒家：人文精神二(East Asian Confucianisms: Humanism (2))](https://www.coursera.org/learn/east-asian-confucianisms-humanism2) National Taiwan University
* [Re-imaging God in Korean Context](https://www.coursera.org/learn/god-korean-context) Yonsei University
* [理解马克思](https://www.coursera.org/learn/ma-ke-si) Nanjing University
* [品读道家的智慧](https://www.coursera.org/learn/daojiao) Xi'an Jiaotong University
* [Mind of the Universe - Genetic Privacy: should we be concerned?](https://www.coursera.org/learn/mind-of-the-universe-genetic-privacy) Universiteit Leiden
* [悖论：思维的魔方](https://www.coursera.org/learn/bei-lun) Peking University
* [《新教伦理与资本主义精神》导读](https://www.coursera.org/learn/max-weber) Fudan University
* [Mind of the Universe: Science in Progress](https://www.coursera.org/learn/mind-of-the-universe-science-in-progress) Erasmus University Rotterdam


## business/business-essentials

* [Introduction to Negotiation: A Strategic Playbook for Becoming a Principled and Persuasive Negotiator](https://www.coursera.org/learn/negotiation) Yale University
* [Gestión Empresarial Exitosa para Pymes](https://www.coursera.org/learn/gestionempresarialpyme) Pontificia Universidad Católica de Chile
* [Fundamentos de Finanzas Empresariales](https://www.coursera.org/learn/finanzas-empresariales) Universidad de los Andes
* [Microeconomics Principles](https://www.coursera.org/learn/microeconomics) University of Illinois at Urbana-Champaign
* [Corporate Finance Essentials](https://www.coursera.org/learn/corporate-finance-essentials) IESE Business School
* [Criação de Startups: Como desenvolver negócios inovadores](https://www.coursera.org/learn/criacao-startups) Universidade de São Paulo
* [Microeconomics: The Power of Markets](https://www.coursera.org/learn/microeconomics-part1) University of Pennsylvania
* [Process Mining: Data science in Action](https://www.coursera.org/learn/process-mining) Eindhoven University of Technology
* [Data Analytics for Lean Six Sigma](https://www.coursera.org/learn/data-analytics-for-lean-six-sigma) University of Amsterdam
* [Supply Chain Analytics](https://www.coursera.org/learn/supply-chain-analytics) Rutgers the State University of New Jersey
* [مقدمة عن التفاوض: دليل استراتيجي لتصبح مُفاوضًا ذا مبادئ ومُقنعًا](https://www.coursera.org/learn/negotiation-ar) Yale University
* [Formulación y evaluación de proyectos complejos](https://www.coursera.org/learn/formulacion-evaluacion-proyectos-ingenieria) Universidad de los Andes
* [Microeconomics: When Markets Fail](https://www.coursera.org/learn/microeconomics-part2) University of Pennsylvania
* [Scaling Operations: Linking Strategy and Execution](https://www.coursera.org/learn/operations-strategy) Northwestern University
* [Keeping up with Change: Issues for the Finance Professional](https://www.coursera.org/learn/change-for-the-finance-professional) University of London
* [Бизнес на свои](https://www.coursera.org/learn/biznes-na-svoi-mosigra) National Research Tomsk State University
* [Emprendiendo en STEM](https://www.coursera.org/learn/emprendiendo-en-stem) Universidad Austral
* [Protecting Business Innovations via Copyright](https://www.coursera.org/learn/protect-business-innovations-copyright) The Hong Kong University of Science and Technology
* [Doing Business in Europe](https://www.coursera.org/learn/doing-business-in-europe) ESCP Business School
* [Працюйте розумніше, а не більше: управління часом для особистої та професійної продуктивності](https://www.coursera.org/learn/upravlinnya-chasom) University of California, Irvine
* [職場素養 (Professionalism)](https://www.coursera.org/learn/zhichang-suyang) National Taiwan University
* [Introduction to Learning Transfer and Life Long Learning (3L)](https://www.coursera.org/learn/intro-learning-transfer) University of California, Irvine
* [Business Model Innovation for Sustainable Landscape Restoration](https://www.coursera.org/learn/bmi-sustainable-landscape-restoration) Erasmus University Rotterdam
* [The Power of Markets I: The Basics of Supply and Demand and Consumer Behavior](https://www.coursera.org/learn/market-power) University of Rochester
* [Teoria Geral da Administração para Executivos](https://www.coursera.org/learn/tga-executivos) Fundação Instituto de Administração
* [Международная информационная безопасность: теория и практика](https://www.coursera.org/learn/international-information-security) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [The Power of Markets II: Market Structure and Firm Behavior](https://www.coursera.org/learn/market-structure) University of Rochester
* [The Power of Markets III: Input Markets and Promoting Efficiency](https://www.coursera.org/learn/market-efficiency) University of Rochester
* [Bases of the law of obligations (The Russian Federation) Part 2](https://www.coursera.org/learn/russian-law-of-obligations-2) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)


## business/business-strategy

* [Model Thinking](https://www.coursera.org/learn/model-thinking) University of Michigan
* [Innovation Management](https://www.coursera.org/learn/innovation-management) Erasmus University Rotterdam
* [Gestão de Operações](https://www.coursera.org/learn/gestao-de-operacoes) Insper
* [Welcome to Game Theory](https://www.coursera.org/learn/game-theory-introduction) The University of Tokyo
* [International Business I](https://www.coursera.org/learn/international-business) University of New Mexico
* [Supply Chain Management: A Learning Perspective](https://www.coursera.org/learn/supply-chain-management) Korea Advanced Institute of Science and Technology(KAIST)
* [Negocios Internacionales I](https://www.coursera.org/learn/negocios-internacionales) University of New Mexico
* [Business Strategies for Emerging Markets](https://www.coursera.org/learn/business-strategies) National Research University Higher School of Economics
* [Capitalismo Consciente](https://www.coursera.org/learn/capitalismo-consciente) Insper
* [Технология ведения международных переговоров](https://www.coursera.org/learn/tekhnologiya-vedeniya-mezhdunarodnykh-peregovorov) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Deep Learning for Business](https://www.coursera.org/learn/deep-learning-business) Yonsei University
* [Микроэкономика (вводный курс)](https://www.coursera.org/learn/mikroekonomika-vvodnyy-kurs) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [الذكاء الاصطناعي للجميع](https://www.coursera.org/learn/ai-for-everyone-ar) deeplearning.ai
* [服務模式的體驗、設計與創新：從痛點到賣點 (Experience, Design, and Innovation of Service Models: from Pain Points to Selling Points)](https://www.coursera.org/learn/service-models) National Taiwan University
* [International Business II](https://www.coursera.org/learn/international-business-2) University of New Mexico
* [Государственно-частное партнерство в инфраструктурном развитии России](https://www.coursera.org/learn/gosudarstvenno-chastnoye-partnerstvo) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Negocios Internacionales II](https://www.coursera.org/learn/negocios-internacionales-2) University of New Mexico
* [商管研究中的賽局分析（一）：通路選擇、合約制定與共享經濟 (Game Theoretic Analysis for Business Research (1))](https://www.coursera.org/learn/gabr) National Taiwan University
* [賽局與產業競爭策略 (Game Theory and Business Strategy)](https://www.coursera.org/learn/game-theory-and-business-strategy) National Taiwan University
* [Research kitchen](https://www.coursera.org/learn/research-kitchen) Ludwig-Maximilians-Universität München (LMU)
* [Bases of the law of obligations (The Russian Federation) Part 1](https://www.coursera.org/learn/russian-law-of-obligations) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [高阶竞争策略（中文版）](https://www.coursera.org/learn/advanced-competitive-strategy-zh) Ludwig-Maximilians-Universität München (LMU)
* [Value Creation: The Carlson-Polizzotto Method](https://www.coursera.org/learn/valuecreation) Northeastern University


## business/entrepreneurship

* [Desarrollo rápido de productos innovadores para mercados emergentes](https://www.coursera.org/learn/innovacion) Tecnológico de Monterrey
* [Consolidando empresas: Estrutura jurídica e financeira](https://www.coursera.org/learn/consolidando-empresas) Universidade de São Paulo
* [3D Printing Software](https://www.coursera.org/learn/3d-printing-software) University of Illinois at Urbana-Champaign
* [Innovation Through Design: Think, Make, Break, Repeat](https://www.coursera.org/learn/innovation-through-design) The University of Sydney
* [O Empreendedorismo e as Competências do Empreendedor](https://www.coursera.org/learn/empreendedorismo) Universidade Estadual de Campinas
* [Crowdfunding](https://www.coursera.org/learn/wharton-crowdfunding) University of Pennsylvania
* [Créer et développer une startup technologique](https://www.coursera.org/learn/startup-technologique) École Polytechnique
* [Emprender la emprendeduría](https://www.coursera.org/learn/emprender) Universitat de Barcelona
* [How to Validate your Startup Idea](https://www.coursera.org/learn/startup-idea) UNSW Sydney (The University of New South Wales)
* [3D Printing Applications](https://www.coursera.org/learn/3d-printing-applications) University of Illinois at Urbana-Champaign
* [Patenting in Biotechnology](https://www.coursera.org/learn/patenting-bio-ipr) Technical University of Denmark (DTU)
* [Local Economic Development](https://www.coursera.org/learn/local-economic-development) Erasmus University Rotterdam
* [Innovative Finance: Hacking finance to change the world](https://www.coursera.org/learn/innovative-finance) University of Cape Town
* [Effectuation : l'entrepreneuriat pour tous](https://www.coursera.org/learn/effectuation) emlyon business school
* [Innovating in a Digital World](https://www.coursera.org/learn/innovating-digital-world) Institut Mines-Télécom
* [L'entrepreneuriat social : de l'envie au projet](https://www.coursera.org/learn/entrepreneuriatquichangelemonde) ESSEC Business School
* [Protecting Business Innovations via Patent](https://www.coursera.org/learn/protect-business-innovations-patent) The Hong Kong University of Science and Technology
* [Beyond Silicon Valley: Growing Entrepreneurship in Transitioning Economies](https://www.coursera.org/learn/entrepreneurship-development) Case Western Reserve University
* [Protecting Business Innovations via Strategy](https://www.coursera.org/learn/protect-business-innovations-strategy) The Hong Kong University of Science and Technology
* [Fundamentals of Sales and Marketing, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-6) Goldman Sachs
* [Grow Your Business with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-1) Goldman Sachs
* [Technology Commercialization, Part 1: Setting up your Idea Filtering System](https://www.coursera.org/learn/technology-commercialization) University of Rochester
* [Fundamentals of Business Finance, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-2) Goldman Sachs
* [Fundamentals of Leadership, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-3) Goldman Sachs
* [The Sun and the Total Eclipse of August 2017](https://www.coursera.org/learn/eclipse) University of Colorado Boulder
* [Fundamentals of Negotiation, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-10) Goldman Sachs
* [Fundamentals of Funding, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-9) Goldman Sachs
* [Fundamentals of Customers and Competition, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-4) Goldman Sachs
* [Fundamentals of Financial Planning, with Goldman Sachs 10,000 Women](https://www.coursera.org/learn/10k-women-5) Goldman Sachs


## business/finance

* [Financial Markets](https://www.coursera.org/learn/financial-markets-global) Yale University
* [Contabilidad para no contadores](https://www.coursera.org/learn/contabilidad) Universidad Nacional Autónoma de México
* [Finanzas personales](https://www.coursera.org/learn/finanzas-personales) Universidad Nacional Autónoma de México
* [Financial Engineering and Risk Management Part I](https://www.coursera.org/learn/financial-engineering-1) Columbia University
* [The Global Financial Crisis](https://www.coursera.org/learn/global-financial-crisis) Yale University
* [Python and Statistics for Financial Analysis](https://www.coursera.org/learn/python-statistics-financial-analysis) The Hong Kong University of Science and Technology
* [Marketing Gerencial](https://www.coursera.org/learn/marketing-gerencial) Universidad de Chile
* [Private Equity and Venture Capital](https://www.coursera.org/learn/private-equity) Università Bocconi
* [Финансовые рынки и институты (Financial Markets and Institutions)](https://www.coursera.org/learn/finansovye-rynki) National Research University Higher School of Economics
* [Administração Financeira](https://www.coursera.org/learn/administracao-financeira) Insper
* [Advanced Valuation and Strategy - M&A, Private Equity, and Venture Capital](https://www.coursera.org/learn/advanced-valuation-and-strategy) Erasmus University Rotterdam
* [Behavioral Finance](https://www.coursera.org/learn/duke-behavioral-finance) Duke University
* [Forensic Accounting and Fraud Examination](https://www.coursera.org/learn/forensic-accounting) West Virginia University
* [Основы корпоративных финансов (Fundamentals of Corporate Finance)](https://www.coursera.org/learn/osnovy-korporativnykh-finansov) National Research University Higher School of Economics
* [Introdução à Análise Macroeconômica](https://www.coursera.org/learn/introducao-analise-macroeconomica) Universidade de São Paulo
* [Financing and Investing in Infrastructure](https://www.coursera.org/learn/infrastructure-investing) Università Bocconi
* [Finanzas Corporativas](https://www.coursera.org/learn/finanzas-corporativas) Universidad Austral
* [Financial Engineering and Risk Management Part II](https://www.coursera.org/learn/financial-engineering-2) Columbia University
* [Das liebe Geld - Finance im Alltag](https://www.coursera.org/learn/finanzen) University of Zurich
* [Economie du sol et de l'immobilier I](https://www.coursera.org/learn/economie-sol-immobilier-1) École Polytechnique Fédérale de Lausanne
* [Public Economics](https://www.coursera.org/learn/public-economics) National Research University Higher School of Economics
* [Budgeting essentials and development](https://www.coursera.org/learn/budgeting-essentials-development) Fundação Instituto de Administração
* [Monetary Policy in the Asia Pacific](https://www.coursera.org/learn/monetary-policy-asia-pacific) The Hong Kong University of Science and Technology
* [Пути выхода на фондовый рынок для частных инвесторов сегмента Mass Retail](https://www.coursera.org/learn/vyhoda-na-fondovyj-rynok-mass-retail) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Налоги и налогообложение: специальные налоговые режимы](https://www.coursera.org/learn/specialnye-nalogovye-rezhimy) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Государственное регулирование финансовых рынков на современном этапе](https://www.coursera.org/learn/gosudarstve-regulirovaniye-finansovykh-rynkov) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Цифровые технологии в международных финансах](https://www.coursera.org/learn/cifrovye-tekhnologii-v-mezhdunarodnyh-finansah) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Фінанси для нефінансових спеціалістів](https://www.coursera.org/learn/finansy) University of California, Irvine
* [Economie du sol et de l'immobilier II](https://www.coursera.org/learn/economie-sol-immobilier-2) École Polytechnique Fédérale de Lausanne


## business/leadership-and-management

* [Camino a la Excelencia en Gestión de Proyectos](https://www.coursera.org/learn/camino-excelencia-gestion-proyectos) Pontificia Universidad Católica de Chile
* [Management of Fashion and Luxury Companies](https://www.coursera.org/learn/mafash) Università Bocconi
* [Managing the Company of the Future](https://www.coursera.org/learn/company-future-management) University of London
* [Food & Beverage Management](https://www.coursera.org/learn/food-beverage-management) Università Bocconi
* [Diseño y Creación de un Emprendimiento Social](https://www.coursera.org/learn/emprendimiento-social-negocios-sustentable-canvas-sociales) Pontificia Universidad Católica de Chile
* [Claves para Gestionar Personas](https://www.coursera.org/learn/gestionar-personas) IESE Business School
* [Gestión de organizaciones efectivas](https://www.coursera.org/learn/gestion-organizaciones-efectivas) Pontificia Universidad Católica de Chile
* [International Leadership and Organizational Behavior](https://www.coursera.org/learn/organizational-behavior) Università Bocconi
* [International Organizations Management](https://www.coursera.org/learn/international-organizations-management) University of Geneva
* [Organizational Analysis](https://www.coursera.org/learn/organizational-analysis) Stanford University
* [Social Impact Strategy: Tools for Entrepreneurs and Innovators](https://www.coursera.org/learn/social-impact) University of Pennsylvania
* [Design-Led Strategy: Design thinking for business strategy and entrepreneurship](https://www.coursera.org/learn/design-strategy) The University of Sydney
* [Les Fondamentaux de la Négociation](https://www.coursera.org/learn/fondamentaux-negociation) ESSEC Business School
* [Arts and Heritage Management](https://www.coursera.org/learn/arts-heritage) Università Bocconi
* [Conceitos Básicos de Logística e Supply Chain](https://www.coursera.org/learn/conceitos-basicos-logistica) Universidade Estadual de Campinas
* [Corporate Sustainability. Understanding and Seizing the Strategic Opportunity](https://www.coursera.org/learn/corp-sustainability) Università Bocconi
* [How to Finance and Grow Your Startup – Without VC](https://www.coursera.org/learn/startup-financing-without-vc) University of London
* [Smart Cities – Management of Smart Urban Infrastructures](https://www.coursera.org/learn/smart-cities) École Polytechnique Fédérale de Lausanne
* [L'excellence opérationnelle en pratique](https://www.coursera.org/learn/excellence-operationnelle) ESSEC Business School
* [Bridging the Gap between Strategy Design and Delivery](https://www.coursera.org/learn/bridging-strategy-design-delivery-gap) Brightline Initiative
* [Gestión de las empresas de alimentación y bebidas](https://www.coursera.org/learn/empresas-alimentos-bebidas) Università Bocconi
* [Buenas Prácticas en Libre Competencia](https://www.coursera.org/learn/libre-competencia) Pontificia Universidad Católica de Chile
* [Administración Estratégica y Emprendedora](https://www.coursera.org/learn/administracion-estrategica) University of New Mexico
* [Raison d’être et Entreprise à Mission](https://www.coursera.org/learn/raison-etre-et-entreprise-a-mission) ESSEC Business School
* [Corporate Strategy](https://www.coursera.org/learn/corporatestrategy) University of London
* [Managing Responsibly: Practicing Sustainability, Responsibility and Ethics](https://www.coursera.org/learn/responsible-management) University of Manchester
* [Management of Urban Infrastructures – part 1](https://www.coursera.org/learn/managing-urban-infrastructures-1) École Polytechnique Fédérale de Lausanne
* [New Technologies for Business Leaders](https://www.coursera.org/learn/new-technologies-business-leaders) Rutgers the State University of New Jersey
* [Diseño de Experiencia en Servicios](https://www.coursera.org/learn/diseno-experiencia-servicios) Universidad Austral
* [Innovative Governance of Large Urban Systems](https://www.coursera.org/learn/iglus) École Polytechnique Fédérale de Lausanne
* [L'innovation managériale en pratique](https://www.coursera.org/learn/innovation-manageriale) ESSEC Business School
* [Accounting, Business and Society: The Multi-faceted Role of Accounting](https://www.coursera.org/learn/accounting-business-society) The Hong Kong University of Science and Technology
* [Population Health: Fundamentals of Population Health Management](https://www.coursera.org/learn/fundamentals-population-health-management) Universiteit Leiden
* [Прикладное управление рисками](https://www.coursera.org/learn/applied-risk-management) National Research Tomsk State University
* [Правовые формы ведения бизнеса в России](https://www.coursera.org/learn/pravovyye-formy-vedeniya-biznesa-rossii) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Moving to the Cloud](https://www.coursera.org/learn/cloud-computing-adoption) The University of Melbourne
* [Leadership d'excellence par le sport de haut niveau](https://www.coursera.org/learn/leadership-excellence-sport) ESSEC Business School
* [Blockchain 360: A State of the Art for Professionals](https://www.coursera.org/learn/blockchain-professionals) EIT Digital
* [إدارة شركات المستقبل](https://www.coursera.org/learn/company-future-management-ar) University of London
* [Теория отраслевых рынков (Industrial Organization)](https://www.coursera.org/learn/otraslevye-rynki) National Research University Higher School of Economics
* [Gestión del alcance: el qué de la triple restricción](https://www.coursera.org/learn/gestion-alcance-proyectos) Universidad de los Andes
* [Entrepreneurial Strategic Management](https://www.coursera.org/learn/entrepreneurial-strategic-management) University of New Mexico
* [A prática da gestão de clubes e federações esportivas](https://www.coursera.org/learn/fia-gestao-clubes-federacoes-esportivas) Fundação Instituto de Administração
* [Power Onboarding](https://www.coursera.org/learn/power-onboarding) Northwestern University
* [Subsistence Marketplaces](https://www.coursera.org/learn/subsistence-marketplaces) University of Illinois at Urbana-Champaign
* [Originalité et modernité du mutualisme](https://www.coursera.org/learn/originalite-et-modernite-du-mutualisme) ESSEC Business School
* [Business Implications of AI: A Nano-course](https://www.coursera.org/learn/business-implications-ai-nano-course) EIT Digital


## business/marketing

* [The Strategy of Content Marketing](https://www.coursera.org/learn/content-marketing) University of California, Davis
* [Brand Management: Aligning Business, Brand and Behaviour](https://www.coursera.org/learn/brand) University of London
* [Costos para los Negocios](https://www.coursera.org/learn/costosparanegocios) Universidad de Chile
* [Introdução ao Marketing Analítico](https://www.coursera.org/learn/marketing-analitico) Insper
* [Sports Marketing](https://www.coursera.org/learn/sports-marketing) Northwestern University
* [Patrocinio Deportivo](https://www.coursera.org/learn/patrocinio-deportivo) Universitat Autònoma de Barcelona
* [Sport Sponsorship. Let them Play](https://www.coursera.org/learn/sport-sponsorship) Universitat Autònoma de Barcelona
* [Transferencia tecnológica: De la investigación al mercado.](https://www.coursera.org/learn/transferencia-tecnologica-investigacion) Pontificia Universidad Católica de Chile
* [Advertising and Society](https://www.coursera.org/learn/role-of-advertising) Duke University
* [Комплекс маркетинга: 5Р](https://www.coursera.org/learn/kompleks-marketinga-5p) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Customer Insights: New Product Development Orientation](https://www.coursera.org/learn/customer-insights-orientation) University of Illinois at Urbana-Champaign
* [Маркетинг инновационных продуктов](https://www.coursera.org/learn/marketing-innov-produktov) Moscow Institute of Physics and Technology
* [Coberturas de riesgo con futuros y opciones para agrobusiness](https://www.coursera.org/learn/coberturas-de-riesgo) Universidad Austral
* [The Olympic Games and the Media](https://www.coursera.org/learn/olympic-games) Universitat Autònoma de Barcelona
* [行銷典範轉移: 變動中的消費世界 (Marketing in a changing world)](https://www.coursera.org/learn/taiwan-marketing-stp-crm) National Taiwan University
* [Макроэкономика (вводный курс)](https://www.coursera.org/learn/makroekonomika) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [Customer Insights: Quantitative Techniques](https://www.coursera.org/learn/quantitative-customer-insights) University of Illinois at Urbana-Champaign
* [Разработка инновационного продукта](https://www.coursera.org/learn/developing-products-new-market) Moscow Institute of Physics and Technology
* [Protecting Business Innovations via Trademark](https://www.coursera.org/learn/protect-business-innovations-trademark) The Hong Kong University of Science and Technology
* [Marketing Internacional en Asia](https://www.coursera.org/learn/marketing-internacional-asia) Yonsei University


## computer-science/algorithms

* [Основы программирования на Python](https://www.coursera.org/learn/python-osnovy-programmirovaniya) National Research University Higher School of Economics
* [Introducción a Data Science: Programación Estadística con R](https://www.coursera.org/learn/intro-data-science-programacion-estadistica-r) Universidad Nacional Autónoma de México
* [Introducción a la Minería de Datos](https://www.coursera.org/learn/mineria-de-datos-introduccion) Pontificia Universidad Católica de Chile
* [Analysis of Algorithms](https://www.coursera.org/learn/analysis-of-algorithms) Princeton University
* [Computer Science: Algorithms, Theory, and Machines](https://www.coursera.org/learn/cs-algorithms-theory-machines) Princeton University
* [Computers, Waves, Simulations: A Practical Introduction to Numerical Methods using Python](https://www.coursera.org/learn/computers-waves-simulations) Ludwig-Maximilians-Universität München (LMU)
* [Detección de objetos](https://www.coursera.org/learn/deteccion-objetos) Universitat Autònoma de Barcelona
* [Clasificación de imágenes: ¿cómo reconocer el contenido de una imagen?](https://www.coursera.org/learn/clasificacion-imagenes) Universitat Autònoma de Barcelona
* [Спортивное программирование](https://www.coursera.org/learn/sportivnoe-programmirovanie) National Research Tomsk State University
* [Approximation Algorithms Part I](https://www.coursera.org/learn/approximation-algorithms-part-1) École normale supérieure
* [人工智慧：搜尋方法與邏輯推論 (Artificial Intelligence - Search & Logic)](https://www.coursera.org/learn/rengong-zhineng) National Taiwan University
* [I/O-efficient algorithms](https://www.coursera.org/learn/io-efficient-algorithms) EIT Digital
* [算法设计与分析 Design and Analysis of Algorithms](https://www.coursera.org/learn/algorithms) Peking University
* [Approximation Algorithms Part II](https://www.coursera.org/learn/approximation-algorithms-part-2) École normale supérieure


## computer-science/computer-security-and-networks

* [Bitcoin and Cryptocurrency Technologies](https://www.coursera.org/learn/cryptocurrency) Princeton University
* [Information Security: Context and Introduction](https://www.coursera.org/learn/information-security-data) University of London
* [Internet History, Technology, and Security](https://www.coursera.org/learn/internet-history) University of Michigan
* [International Cyber Conflicts](https://www.coursera.org/learn/cyber-conflicts) The State University of New York
* [Networks: Friends, Money, and Bytes](https://www.coursera.org/learn/friends-money-bytes) Princeton University
* [Введение в искусственный интеллект](https://www.coursera.org/learn/vvedenie-v-iskusstvennyi-intellekt) National Research Tomsk State University
* [计算机组成 Computer Organization](https://www.coursera.org/learn/jisuanji-zucheng) Peking University
* [Networks Illustrated: Principles without Calculus](https://www.coursera.org/learn/networks-illustrated) Princeton University
* [Securing Digital Democracy](https://www.coursera.org/learn/digital-democracy) University of Michigan
* [操作系统与虚拟化安全](https://www.coursera.org/learn/os-virtsecurity) Peking University


## computer-science/design-and-product

* [Processamento Digital de Sinais - Amostragem](https://www.coursera.org/learn/pds) Universidade Estadual de Campinas


## computer-science/mobile-and-web-development

* [Programming Languages, Part A](https://www.coursera.org/learn/programming-languages) University of Washington
* [Control of Mobile Robots](https://www.coursera.org/learn/mobile-robot) Georgia Institute of Technology
* [Introduction to Augmented Reality and ARCore](https://www.coursera.org/learn/ar) Google AR & VR
* [Developing Android Apps with App Inventor](https://www.coursera.org/learn/app-inventor-android) The Hong Kong University of Science and Technology
* [Programming Mobile Applications for Android Handheld Systems: Part 1](https://www.coursera.org/learn/android-programming) University of Maryland, College Park
* [Introdução ao Desenvolvimento de Aplicativos Android](https://www.coursera.org/learn/introducao-aplicativos-android) Universidade Estadual de Campinas
* [Programming Languages, Part B](https://www.coursera.org/learn/programming-languages-part-b) University of Washington
* [Programming Languages, Part C](https://www.coursera.org/learn/programming-languages-part-c) University of Washington
* [Programming Mobile Applications for Android Handheld Systems: Part 2](https://www.coursera.org/learn/android-programming-2) University of Maryland, College Park
* [软件测试 (Software Testing)](https://www.coursera.org/learn/ruanjian-ceshi) Nanjing University


## computer-science/software-development

* [Algorithms, Part I](https://www.coursera.org/learn/algorithms-part1) Princeton University
* [Introduction to Programming with MATLAB](https://www.coursera.org/learn/matlab) Vanderbilt University
* [Learn to Program: The Fundamentals](https://www.coursera.org/learn/learn-to-program) University of Toronto
* [Introdução à Ciência da Computação com Python Parte 1](https://www.coursera.org/learn/ciencia-computacao-python-conceitos) Universidade de São Paulo
* [Code Yourself! An Introduction to Programming](https://www.coursera.org/learn/intro-programming) The University of Edinburgh
* [Introducción a Java](https://www.coursera.org/learn/introduccion-java) Universidad Nacional Autónoma de México
* [Introduction to Logic](https://www.coursera.org/learn/logic-introduction) Stanford University
* [Computer Science: Programming with a Purpose](https://www.coursera.org/learn/cs-programming-java) Princeton University
* [C for Everyone: Programming Fundamentals](https://www.coursera.org/learn/c-for-everyone) University of California, Santa Cruz
* [Biology Meets Programming: Bioinformatics for Beginners](https://www.coursera.org/learn/bioinformatics) University of California San Diego
* [Algorithms, Part II](https://www.coursera.org/learn/algorithms-part2) Princeton University
* [Agile with Atlassian Jira](https://www.coursera.org/learn/agile-atlassian-jira) Atlassian
* [Python Programming: A Concise Introduction](https://www.coursera.org/learn/python-programming-introduction) Wesleyan University
* [¡A Programar! Una introducción a la programación](https://www.coursera.org/learn/a-programar) Universidad ORT Uruguay
* [The Unix Workbench](https://www.coursera.org/learn/unix) Johns Hopkins University
* [The Finite Element Method for Problems in Physics](https://www.coursera.org/learn/finite-element-method) University of Michigan
* [Software Defined Networking](https://www.coursera.org/learn/sdn) The University of Chicago
* [用 Python 做商管程式設計（一）(Programming for Business Computing in Python (1))](https://www.coursera.org/learn/pbc1) National Taiwan University
* [Interactive Computer Graphics](https://www.coursera.org/learn/interactive-computer-graphics) The University of Tokyo
* [Image and Video Processing: From Mars to Hollywood with a Stop at the Hospital](https://www.coursera.org/learn/image-processing) Duke University
* [Problem Solving, Python Programming, and Video Games](https://www.coursera.org/learn/problem-solving-programming-video-games) University of Alberta
* [Introduction à la programmation orientée objet (en C++)](https://www.coursera.org/learn/programmation-orientee-objet-cpp) École Polytechnique Fédérale de Lausanne
* [Audio Signal Processing for Music Applications](https://www.coursera.org/learn/audio-signal-processing) Universitat Pompeu Fabra of Barcelona
* [Документы и презентации в LaTeX (Introduction to LaTeX)](https://www.coursera.org/learn/latex) National Research University Higher School of Economics
* [Introdução ao Teste de Software](https://www.coursera.org/learn/intro-teste-de-software) Universidade de São Paulo
* [Initiation à la programmation (en C++)](https://www.coursera.org/learn/initiation-programmation-cpp) École Polytechnique Fédérale de Lausanne
* [Introdução à Ciência da Computação com Python Parte 2](https://www.coursera.org/learn/ciencia-computacao-python-conceitos-2) Universidade de São Paulo
* [Data Processing Using Python](https://www.coursera.org/learn/python-data-processing) Nanjing University
* [Initiation à la programmation (en Java)](https://www.coursera.org/learn/initiation-programmation-java) École Polytechnique Fédérale de Lausanne
* [Learn to Program: Crafting Quality Code](https://www.coursera.org/learn/program-code) University of Toronto
* [操作系统原理（Operating Systems）](https://www.coursera.org/learn/os-pku) Peking University
* [用Python玩转数据 Data Processing Using Python](https://www.coursera.org/learn/hipython) Nanjing University
* [Introduction à la programmation orientée objet (en Java)](https://www.coursera.org/learn/programmation-orientee-objet-java) École Polytechnique Fédérale de Lausanne
* [Basic Modeling for Discrete Optimization](https://www.coursera.org/learn/basic-modeling) The University of Melbourne
* [用 Python 做商管程式設計（二）(Programming for Business Computing in Python (2))](https://www.coursera.org/learn/pbc2) National Taiwan University
* [Architecting Smart IoT Devices](https://www.coursera.org/learn/iot-architecture) EIT Digital
* [Introduction to Architecting Smart IoT Devices](https://www.coursera.org/learn/iot-devices) EIT Digital
* [Programming with Cloud IoT Platforms](https://www.coursera.org/learn/cloud-iot-platform) Pohang University of Science and Technology
* [計算機程式設計 (Computer Programming)](https://www.coursera.org/learn/c-bian-cheng) National Taiwan University
* [Software Architecture for the Internet of Things](https://www.coursera.org/learn/iot-software-architecture) EIT Digital
* [Introduction to OpenCL on FPGAs](https://www.coursera.org/learn/opencl-fpga-introduction) Intel
* [Creative Programming for Digital Media & Mobile Apps](https://www.coursera.org/learn/digitalmedia) University of London
* [用 Python 做商管程式設計（三）(Programming for Business Computing in Python (3))](https://www.coursera.org/learn/pbc3) National Taiwan University
* [Java程序设计](https://www.coursera.org/learn/java-chengxu-sheji) Peking University
* [Projet de programmation (en Java)](https://www.coursera.org/learn/projet-programmation-java) École Polytechnique Fédérale de Lausanne
* [C#程序设计](https://www.coursera.org/learn/sheng-c-biancheng) Peking University
* [Advanced Modeling for Discrete Optimization](https://www.coursera.org/learn/advanced-modeling) The University of Melbourne
* [Solving Algorithms for Discrete Optimization](https://www.coursera.org/learn/solving-algorithms-discrete-optimization) The University of Melbourne
* [Введение в параллельное программирование с использованием OpenMP и MPI](https://www.coursera.org/learn/parallelnoye-programmirovaniye) National Research Tomsk State University
* [Hands-on Text Mining and Analytics](https://www.coursera.org/learn/text-mining-analytics) Yonsei University
* [System Validation: Automata and behavioural equivalences](https://www.coursera.org/learn/automata-system-validation) EIT Digital
* [Expanded FPGA Training with NIOS II](https://www.coursera.org/learn/fpga-training-nios-ii) University of Colorado Boulder
* [Использование механизмов операционных систем в разработке программного обеспечения](https://www.coursera.org/learn/os-v-razrabotke-po) National Research Nuclear University MEPhI
* [Разработка корпоративных систем. Часть 2. Строгие методологии разработки](https://www.coursera.org/learn/strogie-metodologii-razrabotki) National Research Nuclear University MEPhI
* [软件工程](https://www.coursera.org/learn/ruanjian-gongcheng) Peking University
* [计算机操作系统](https://www.coursera.org/learn/jisuanji-caozuo-xitong) Nanjing University
* [Quantitative Model Checking](https://www.coursera.org/learn/quantitative-model-checking) EIT Digital
* [Разработка корпоративных систем. Часть 3. Гибкие методологии разработки](https://www.coursera.org/learn/gibkie-metodologii-razrabotki) National Research Nuclear University MEPhI
* [离散优化建模基础篇 Basic Modeling for Discrete Optimization](https://www.coursera.org/learn/lisan-youhua-jianmo-jichupian) The Chinese University of Hong Kong
* [Методологии антикризисного жизненного цикла корпоративных систем](https://www.coursera.org/learn/korporativnye-antikrizisnye-methodology) National Research Nuclear University MEPhI
* [Quantitative Formal Modeling and Worst-Case Performance Analysis](https://www.coursera.org/learn/quantitative-formal-modeling-1) EIT Digital
* [Разработка корпоративных систем. Часть 1. Модели жизненного цикла](https://www.coursera.org/learn/razrabotka-korporativnih-sistem-modeli-jiznennogo-cikla) National Research Nuclear University MEPhI
* [面向对象技术高级课程（The Advanced Object-Oriented Technology）](https://www.coursera.org/learn/aoo) Peking University
* [System Validation (2): Model process behaviour](https://www.coursera.org/learn/system-validation-behavior) EIT Digital
* [System Validation (4): Modelling Software, Protocols, and other behaviour](https://www.coursera.org/learn/system-validation-software-protocols) EIT Digital
* [离散优化算法篇 Solving Algorithms for Discrete Optimization](https://www.coursera.org/learn/lisan-youhua-suanfapian) The Chinese University of Hong Kong
* [系统平台与计算环境](https://www.coursera.org/learn/jisuanji-wangluo) Xi'an Jiaotong University
* [离散优化建模高阶篇 Advanced Modeling for Discrete Optimization](https://www.coursera.org/learn/lisan-youhua-jianmo-gaojiepian) The Chinese University of Hong Kong


## data-science/data-analysis

* [Fundamentos de Excel para Negocios](https://www.coursera.org/learn/excel-para-negocios) Universidad Austral
* [Excel aplicado a los negocios (Nivel Avanzado)](https://www.coursera.org/learn/excel-aplicado-negocios-avanzado) Universidad Austral
* [Social and Economic Networks: Models and Analysis](https://www.coursera.org/learn/social-economic-networks) Stanford University
* [Econometria Básica Aplicada](https://www.coursera.org/learn/econometria-basica-aplicada) Universidade de São Paulo
* [Data-driven Astronomy](https://www.coursera.org/learn/data-driven-astronomy) The University of Sydney
* [Hadoop Platform and Application Framework](https://www.coursera.org/learn/hadoop) University of California San Diego
* [Foundations of Data Science: K-Means Clustering in Python](https://www.coursera.org/learn/data-science-k-means-clustering-python) University of London
* [大數據分析：商業應用與策略管理 (Big Data Analytics: Business Applications and Strategic Decisions)](https://www.coursera.org/learn/bigdataanalysis) National Taiwan University
* [Population Health: Predictive Analytics](https://www.coursera.org/learn/population-health-predictive-analytics) Universiteit Leiden
* [Ecology: from cells to Gaia](https://www.coursera.org/learn/ecology) National Research Tomsk State University
* [Data Science Ethics](https://www.coursera.org/learn/data-science-ethics) University of Michigan
* [A Scientific Approach to Innovation Management](https://www.coursera.org/learn/scientific-approach-innovation-management) Università Bocconi
* [Understanding China, 1700-2000: A Data Analytic Approach, Part 1](https://www.coursera.org/learn/understanding-china-history-part-1) The Hong Kong University of Science and Technology
* [Structural Equation Model and its Applications ]( 结构方程模型及其应用 (普通话)) https://www.coursera.org/learn/jiegou-fangcheng-moxing
* [مقدمة عن البيانات الضخمة](https://www.coursera.org/learn/big-data-introduction-ar) University of California San Diego
* [Global Statistics - Composite Indices for International Comparisons](https://www.coursera.org/learn/global-statistics) University of Geneva
* [Structural Equation Model and its Applications ]( 结构方程模型及其应用 (粤语)) https://www.coursera.org/learn/structural-equation-model-cantonese
* [Understanding China, 1700-2000: A Data Analytic Approach, Part 2](https://www.coursera.org/learn/understanding-china-history-part-2) The Hong Kong University of Science and Technology


## data-science/machine-learning

* [Machine Learning](https://www.coursera.org/learn/machine-learning) Stanford University
* [Введение в машинное обучение](https://www.coursera.org/learn/vvedenie-mashinnoe-obuchenie) National Research University Higher School of Economics
* [機器學習基石上 (Machine Learning Foundations)---Mathematical Foundations](https://www.coursera.org/learn/ntumlone-mathematicalfoundations) National Taiwan University
* [The Development of Mobile Health Monitoring Systems](https://www.coursera.org/learn/mobile-health-monitoring-systems) Saint Petersburg State University
* [機器學習技法 (Machine Learning Techniques)](https://www.coursera.org/learn/machine-learning-techniques) National Taiwan University
* [機器學習基石下 (Machine Learning Foundations)---Algorithmic Foundations](https://www.coursera.org/learn/ntumlone-algorithmicfoundations) National Taiwan University
* [人工智慧：機器學習與理論基礎 (Artificial Intelligence - Learning & Theory)](https://www.coursera.org/learn/ai2) National Taiwan University


## data-science/probability-and-statistics

* [Estadística aplicada a los negocios](https://www.coursera.org/learn/estadistica-aplicada-negocios) Universidad Austral
* [Методология научных исследований и котики](https://www.coursera.org/learn/metodologiya-nauchnyh-issledovanij-kotiki) National Research Tomsk State University
* [Experimentation for Improvement](https://www.coursera.org/learn/experimentation) McMaster University
* [Improving Your Statistical Questions](https://www.coursera.org/learn/improving-statistical-questions) Eindhoven University of Technology


## information-technology/cloud-computing

* [Introduction and Programming with IoT Boards](https://www.coursera.org/learn/introduction-iot-boards) Pohang University of Science and Technology
* [Blockchain for the decision maker](https://www.coursera.org/learn/blockchain-decision-maker) EIT Digital
* [Google Cloud Fundamentals for Azure Professionals: Core Infrastructure](https://www.coursera.org/learn/gcp-fundamentals-azure) Google Cloud
* [Optimizing Your Google Cloud Platform (GCP) Costs](https://www.coursera.org/learn/gcp-cost-optimization) Google Cloud
* [Preparing for the Google Cloud Professional Cloud Architect Exam em Português Brasileiro](https://www.coursera.org/learn/preparing-cloud-professional-cloud-architect-exam-br) Google Cloud


## information-technology/data-management

* [Mastering Digital Twins](https://www.coursera.org/learn/mastering-digital-twins) EIT Digital


## information-technology/networking

* [Сетевое администрирование: от теории к практике](https://www.coursera.org/learn/network-administration) National Research Tomsk State University
* [Intel® Network Academy - Network Transformation 101](https://www.coursera.org/learn/network-transformation-101) Intel


## information-technology/security

* [Information Systems Auditing, Controls and Assurance](https://www.coursera.org/learn/information-systems-audit) The Hong Kong University of Science and Technology
* [International Security Management](https://www.coursera.org/learn/international-security-management) Erasmus University Rotterdam
* [Cybersecurity Awareness and Innovation](https://www.coursera.org/learn/cybersecurity) EIT Digital
* [Security Awareness Training](https://www.coursera.org/learn/security-awareness-training) (ISC)²
* [Security and Privacy for Big Data - Part 2](https://www.coursera.org/learn/security-privacy-big-data-protection) EIT Digital


## language-learning/learning-english

* [English for Career Development](https://www.coursera.org/learn/careerdevelopment) University of Pennsylvania
* [English for Business and Entrepreneurship](https://www.coursera.org/learn/business) University of Pennsylvania
* [English for Journalism](https://www.coursera.org/learn/journalism) University of Pennsylvania
* [English Composition I](https://www.coursera.org/learn/english-composition) Duke University
* [Writing in English at University](https://www.coursera.org/learn/writing-english-university) Lund University
* [Lesson ]( Small Talk & Conversational Vocabulary) https://www.coursera.org/learn/lesson-small-talk-and-conversational-vocabulary
* [Lesson ]( Business English Skills: How to Write Effective Openings and Closings to Emails) https://www.coursera.org/learn/lesson-business-english-skills-how-to-write-effective-openings-and-closings-to-emails
* [Lesson ]( Express Yourself: Pronunciation) https://www.coursera.org/learn/lesson-express-yourself-pronunciation
* [Writing for Young Readers: Opening the Treasure Chest](https://www.coursera.org/learn/writing-for-children) Commonwealth Education Trust
* [Translation in Practice](https://www.coursera.org/learn/translation-in-practice) Nanjing University
* [Lesson ]( Business English Skills: Introducing Yourself in Business Settings) https://www.coursera.org/learn/lesson-business-english-skills-introducing-yourself-in-business-settings
* [Lesson ]( Get Ready for the Interview) https://www.coursera.org/learn/lesson-get-ready-for-the-interview
* [Lesson ]( Video Conferencing: Face to Face but Online) https://www.coursera.org/learn/lesson-video-conferencing-face-to-face-but-online
* [Lesson ]( Telephone Language) https://www.coursera.org/learn/lesson-telephone-language
* [Lesson ]( Business English Skills: How to Navigate Tone, Formality, and Directness in Emails) https://www.coursera.org/learn/business-english-skills-how-to-navigate-tone-formality-directness-in-emails
* [خيارات لسانية لمحترفي الإعلام باللغة العربية](https://www.coursera.org/learn/arabic-for-media) Northwestern University
* [Lesson ]( Understand and Be Understood on the Phone) https://www.coursera.org/learn/lesson-understand-and-be-understood-on-the-phone
* [Lesson ]( Organize Your Pitch) https://www.coursera.org/learn/lesson-organize-your-pitch
* [计算机辅助翻译原理与实践 Principles and Practice of Computer-Aided Translation](https://www.coursera.org/learn/fanyi-ruanjian) Peking University


## language-learning/other-languages

* [Chinese for Beginners](https://www.coursera.org/learn/learn-chinese) Peking University
* [First Step Korean](https://www.coursera.org/learn/learn-korean) Yonsei University
* [Étudier en France: French Intermediate course B1-B2](https://www.coursera.org/learn/etudier-en-france) École Polytechnique
* [Greek and Roman Mythology](https://www.coursera.org/learn/mythology) University of Pennsylvania
* [Fundamentos de la escritura](https://www.coursera.org/learn/escritura-esp) Tecnológico de Monterrey
* [Learn to Speak Korean 1](https://www.coursera.org/learn/learn-speak-korean1) Yonsei University
* [Miracles of Human Language: An Introduction to Linguistics](https://www.coursera.org/learn/human-language) Universiteit Leiden
* [Corrección, estilo y variaciones de la lengua española](https://www.coursera.org/learn/correccion-estilo-variaciones) Universitat Autònoma de Barcelona
* [Fundamentos de la escritura académica](https://www.coursera.org/learn/escritura-academica-esp) Tecnológico de Monterrey
* [Chinese Characters for beginner 汉字](https://www.coursera.org/learn/hanzi) Peking University
* [Spanish for Successful Communication in Healthcare Settings](https://www.coursera.org/learn/spanish-in-healthcare-settings) Rice University
* [Chinese for HSK 4](https://www.coursera.org/learn/hsk-4) Peking University
* [Learning Chinese : Start From Scratch (零到一學中文)](https://www.coursera.org/learn/learn-chinese-mandarin) National Taiwan University
* [Chinese for HSK 5](https://www.coursera.org/learn/chinese-for-hsk5) Peking University
* [Pluralidades em Português Brasileiro](https://www.coursera.org/learn/brasileiro-portugues) Universidade Estadual de Campinas
* [Я говорю по-русски/ I speak Russian](https://www.coursera.org/learn/ya-govoryu-po-russki) National Research Tomsk State University
* [Chinese for HSK 6](https://www.coursera.org/learn/chinese-for-hsk-6) Peking University
* [More Chinese for Beginners](https://www.coursera.org/learn/more-chinese-for-beginners) Peking University
* [Русский язык как инструмент успешной коммуникации](https://www.coursera.org/learn/russian) National Research Tomsk State University
* [Business Chinese 1 中级汉语 （上）](https://www.coursera.org/learn/intermediate-business-chinese-1) Shanghai Jiao Tong University
* [现代汉语核心语法](https://www.coursera.org/learn/hanyu-yufa) Peking University
* [是誰在說話 -- 可愛的臺灣。（Intermediate Chinese）](https://www.coursera.org/learn/learn-intermediate-chinese-mandarin) National Taiwan University
* [中级商务汉语（入职与营销篇）](https://www.coursera.org/learn/business-chinese) Peking University
* [Читаем русскую классику вместе. М. Булгаков «Мастер и Маргарита»](https://www.coursera.org/learn/bulgakov-master-i-margarita) National Research Tomsk State University
* [Towards language universals through lexical semantics: introduction to lexical and semantic typology](https://www.coursera.org/learn/lexical-semantic-typology) National Research University Higher School of Economics
* [Akademiskt skrivande](https://www.coursera.org/learn/akademiskt-skrivande) Lund University
* [Активные процессы в современном русском языке](https://www.coursera.org/learn/aktivnyye-protsessy-sovremennom-russkom-yazyke) National Research Tomsk State University
* [中级商务汉语——商务活动篇](https://www.coursera.org/learn/intermediatechinesebusiness) Peking University
* [Chinese Characters for beginner (2) 汉字(2)](https://www.coursera.org/learn/hanzi-2) Peking University
* [Зарисовки о Сибири. Город Томск: курс русского языка для иностранцев](https://www.coursera.org/learn/zarisovki-o-sibiri) National Research Tomsk State University
* [Взаимодействие языков и культур: сохраняем и расширяем свою идентичность (на примере изучения татарского языка как родного и иностранного)](https://www.coursera.org/learn/tatar-language-and-culture) National Research Tomsk State University


## life-sciences/animal-health

* [Dog Emotion and Cognition](https://www.coursera.org/learn/dog-emotion-and-cognition) Duke University
* [Animal Behaviour and Welfare](https://www.coursera.org/learn/animal-welfare) The University of Edinburgh
* [EDIVET: Do you have what it takes to be a veterinarian?](https://www.coursera.org/learn/becoming-a-veterinarian) The University of Edinburgh
* [The Truth About Cats and Dogs](https://www.coursera.org/learn/cats-and-dogs) The University of Edinburgh
* [Bugs 101: Insect-Human Interactions](https://www.coursera.org/learn/bugs-101) University of Alberta
* [The Horse Course: Introduction to Basic Care and Management](https://www.coursera.org/learn/horse-care) University of Florida
* [Dairy Production and Management](https://www.coursera.org/learn/dairy-production) The Pennsylvania State University
* [Chicken Behaviour and Welfare](https://www.coursera.org/learn/chickens) The University of Edinburgh
* [Sustainable Food Production Through Livestock Health Management](https://www.coursera.org/learn/livestock-farming) University of Illinois at Urbana-Champaign


## life-sciences/basic-science

* [Introductory Human Physiology](https://www.coursera.org/learn/physiology) Duke University
* [Anatomy of the Chest, Abdomen, and Pelvis](https://www.coursera.org/learn/trunk-anatomy) Yale University
* [Understanding the Brain: The Neurobiology of Everyday Life](https://www.coursera.org/learn/neurobiology) The University of Chicago
* [Positive Psychiatry and Mental Health](https://www.coursera.org/learn/positive-psychiatry) The University of Sydney
* [Epidemics - the Dynamics of Infectious Diseases](https://www.coursera.org/learn/epidemics) The Pennsylvania State University
* [Introduction to Genetics and Evolution](https://www.coursera.org/learn/genetics-evolution) Duke University
* [Introduction to Dental Medicine](https://www.coursera.org/learn/dental-medicine-penn) University of Pennsylvania
* [Understanding Plants - Part I: What a Plant Knows](https://www.coursera.org/learn/plantknows) Tel Aviv University
* [Introduction to Forensic Science](https://www.coursera.org/learn/forensic-science) Nanyang Technological University, Singapore
* [Introduction to Breast Cancer](https://www.coursera.org/learn/breast-cancer-causes-prevention) Yale University
* [Dino 101: Dinosaur Paleobiology](https://www.coursera.org/learn/dino101) University of Alberta
* [Industrial Biotechnology](https://www.coursera.org/learn/industrial-biotech) University of Manchester
* [Implant Dentistry](https://www.coursera.org/learn/implant-dentistry) The University of Hong Kong
* [Fundamental Neuroscience for Neuroimaging](https://www.coursera.org/learn/neuroscience-neuroimaging) Johns Hopkins University
* [Ecology: Ecosystem Dynamics and Conservation](https://www.coursera.org/learn/ecology-conservation) American Museum of Natural History
* [The Oral Cavity: Portal to Health and Disease](https://www.coursera.org/learn/oralcavity) University of Pennsylvania
* [Everyday Chinese Medicine](https://www.coursera.org/learn/everyday-chinese-medicine) The Chinese University of Hong Kong
* [Основы вирусологии (Introduction to Virology)](https://www.coursera.org/learn/nsu-virology) Novosibirsk State University
* [Anatomy of the Abdomen and Pelvis; a journey from basis to clinic.](https://www.coursera.org/learn/abdomen-anatomy) Universiteit Leiden
* [Epigenetic Control of Gene Expression](https://www.coursera.org/learn/epigenetics) The University of Melbourne
* [Química, guerra y ética](https://www.coursera.org/learn/quimica-etica) Universidad Nacional Autónoma de México
* [Charles Darwin: El origen del evolucionismo moderno](https://www.coursera.org/learn/darwin-origen-evolucionismo-moderno) Universidad Nacional Autónoma de México
* [The Science of Stem Cells](https://www.coursera.org/learn/stem-cells) American Museum of Natural History
* [Генетика (Genetics)](https://www.coursera.org/learn/nsu-genetics) Novosibirsk State University
* [Antimicrobial resistance - theory and methods](https://www.coursera.org/learn/antimicrobial-resistance) Technical University of Denmark (DTU)
* [Osteoarchaeology: The Truth in Our Bones](https://www.coursera.org/learn/truthinourbones-osteoarchaeology-archaeology) Universiteit Leiden
* [Synapses, Neurons and Brains](https://www.coursera.org/learn/synapses) Hebrew University of Jerusalem
* [Advanced Neurobiology I](https://www.coursera.org/learn/advanced-neurobiology1) Peking University
* [Clinical Epidemiology](https://www.coursera.org/learn/clinical-epidemiology) Utrecht University
* [Understanding Plants - Part II: Fundamentals of Plant Biology](https://www.coursera.org/learn/plant-biology) Tel Aviv University
* [From Disease to Genes and Back](https://www.coursera.org/learn/disease-genes) Novosibirsk State University
* [Paleontology: Ancient Marine Reptiles](https://www.coursera.org/learn/ancient-marine-reptiles) University of Alberta
* [Introduction to Reproduction](https://www.coursera.org/learn/reproductive-health) Northwestern University
* [Tropical Parasitology: Protozoans, Worms, Vectors and Human Diseases](https://www.coursera.org/learn/parasitology) Duke University
* [Organ Donation: From Death to Life](https://www.coursera.org/learn/organ-donation) University of Cape Town
* [Paleontology: Theropod Dinosaurs and the Origin of Birds](https://www.coursera.org/learn/theropods-birds) University of Alberta
* [Thoracic Oncology](https://www.coursera.org/learn/thoracic-oncology) University of Michigan
* [Chimpanzee Behavior and Conservation](https://www.coursera.org/learn/chimp) Duke University
* [Paleontology: Early Vertebrate Evolution](https://www.coursera.org/learn/early-vertebrate-evolution) University of Alberta
* [Visual Perception and the Brain](https://www.coursera.org/learn/visual-perception) Duke University
* [Metagenomics applied to surveillance of pathogens and antimicrobial resistance](https://www.coursera.org/learn/metagenomics) Technical University of Denmark (DTU)
* [Classical papers in molecular genetics](https://www.coursera.org/learn/papers-molecular-genetics) University of Geneva
* [Toxicology 21: Scientific Applications](https://www.coursera.org/learn/toxicology-21) Johns Hopkins University
* [Foundations of International Psychiatry](https://www.coursera.org/learn/international-psychiatry) The University of Melbourne
* [Circadian clocks: how rhythms structure life](https://www.coursera.org/learn/circadian-clocks) Ludwig-Maximilians-Universität München (LMU)
* [Evolution Today](https://www.coursera.org/learn/evolution-today) Universiteit Leiden
* [Ecosystems of California](https://www.coursera.org/learn/california-ecosystems) University of California, Santa Cruz
* [结构生物化学（Structural Biochemistry)](https://www.coursera.org/learn/shengwu-huaxue) Nanjing University
* [Evidence-based Toxicology](https://www.coursera.org/learn/evidence-based-toxicology) Johns Hopkins University
* [Genetics and Society: A Course for Educators](https://www.coursera.org/learn/genetics-society) American Museum of Natural History
* [Advanced Neurobiology II](https://www.coursera.org/learn/advancedneurobiologyii) Peking University
* [生物学概念与途径](https://www.coursera.org/learn/biologyconcept) Peking University
* [人体生理学导论（中文版）](https://www.coursera.org/learn/sheng-li-xue) Duke University
* [The Changing Arctic](https://www.coursera.org/learn/changing-arctic) National Research Tomsk State University
* [流行病学基础（上）](https://www.coursera.org/learn/liuxing-bing-xue) Peking University


## life-sciences/healthcare-management

* [Saúde Baseada em Evidências](https://www.coursera.org/learn/sbe) Universidade Estadual de Campinas
* [Leading Healthcare Quality and Safety](https://www.coursera.org/learn/quality-healthcare) The George Washington University
* [eHealth: More than just an electronic record](https://www.coursera.org/learn/ehealth) The University of Sydney
* [Health Care IT: Challenges and Opportunities](https://www.coursera.org/learn/healthcare-it) Icahn School of Medicine at Mount Sinai
* [Clinical Data Models and Data Quality Assessments](https://www.coursera.org/learn/clinical-data-models-and-data-quality-assessments) University of Colorado System
* [The Science of Health Care Delivery](https://www.coursera.org/learn/science-healthcare-delivery) Arizona State University
* [Business Models for Innovative Care for Older People](https://www.coursera.org/learn/business-models-innovative-care) University of Copenhagen
* [Population Health: Alternative Payment Models](https://www.coursera.org/learn/alternative-payment-models) Universiteit Leiden
* [Regulated Competition in Healthcare Systems: Theory & Practice](https://www.coursera.org/learn/regulated-competition-healthcare-systems) Erasmus University Rotterdam


## life-sciences/health-informatics

* [Computational Neuroscience](https://www.coursera.org/learn/computational-neuroscience) University of Washington
* [Bioinformatics: Introduction and Methods 生物信息学: 导论与方法](https://www.coursera.org/learn/bioinformatics-pku) Peking University
* [Principles of fMRI 1](https://www.coursera.org/learn/functional-mri) Johns Hopkins University
* [Introduction to Clinical Data Science](https://www.coursera.org/learn/introduction-clinical-data-science) University of Colorado System
* [Data Science in Stratified Healthcare and Precision Medicine](https://www.coursera.org/learn/datascimed) The University of Edinburgh
* [Introduction to Neurohacking In R](https://www.coursera.org/learn/neurohacking) Johns Hopkins University
* [Clinical Natural Language Processing](https://www.coursera.org/learn/clinical-natural-language-processing) University of Colorado System
* [Population Health: Responsible Data Analysis](https://www.coursera.org/learn/responsible-data-analysis) Universiteit Leiden
* [医学统计学与SPSS软件（基础篇）](https://www.coursera.org/learn/spss-ruanjian) Peking University
* [生物信息学: 导论与方法](https://www.coursera.org/learn/sheng-wu-xin-xi-xue) Peking University
* [Principles of fMRI 2](https://www.coursera.org/learn/functional-mri-2) Johns Hopkins University


## life-sciences/nutrition

* [Stanford Introduction to Food and Health](https://www.coursera.org/learn/food-and-health) Stanford University
* [Nutrición y obesidad: control de sobrepeso](https://www.coursera.org/learn/nutricion-obesidad-sobrepeso) Universidad Nacional Autónoma de México
* [Child Nutrition and Cooking](https://www.coursera.org/learn/childnutrition) Stanford University
* [Actualización en el manejo del paciente con diabetes mellitus tipo 2](https://www.coursera.org/learn/actualizacion-manejo-diabetes-tipo-2) Universidad Nacional Autónoma de México
* [Agricultura urbana y periurbana](https://www.coursera.org/learn/agricultura-urbana) Universidad Nacional Autónoma de México
* [Nutrition and Lifestyle in Pregnancy](https://www.coursera.org/learn/nutrition-pregnancy) Ludwig-Maximilians-Universität München (LMU)
* [Молекулярная диетология: гены, еда и здоровье](https://www.coursera.org/learn/molekulyarnaya-dietologiya) National Research Tomsk State University
* [Innovación agroalimentaria](https://www.coursera.org/learn/innovacion-agro) Universidad Nacional Autónoma de México
* [Understanding Obesity](https://www.coursera.org/learn/understanding-obesity) The University of Edinburgh
* [Seguridad agroalimentaria](https://www.coursera.org/learn/seguridad-alimentaria) Universidad Nacional Autónoma de México
* [Diabetes – the Essential Facts](https://www.coursera.org/learn/diabetes-essential-facts) University of Copenhagen
* [Alimentación y dietética para una vuelta al mundo a vela](https://www.coursera.org/learn/alimentacion-vuelta-al-mundo) Universitat de Barcelona
* [The New Nordic Diet - from Gastronomy to Health](https://www.coursera.org/learn/new-nordic-diet) University of Copenhagen
* [食品安全與毒理 (Food Safety & Toxicology)](https://www.coursera.org/learn/shipin-anquan) National Taiwan University
* [ГМО: технологии создания и применение](https://www.coursera.org/learn/gmo) Novosibirsk State University
* [食品安全與風險分析（Food Safety＆Risk Analysis）](https://www.coursera.org/learn/foodsafety2) National Taiwan University


## life-sciences/patient-care

* [Farmacología para odontólogos](https://www.coursera.org/learn/farmaco-odontologos) Universidad Nacional Autónoma de México
* [Cuidado de heridas en el ámbito hospitalario](https://www.coursera.org/learn/cuidado-heridas) Universidad Nacional Autónoma de México
* [Atención Primaria en Salud: El desafío de las Enfermedades no Transmisibles](https://www.coursera.org/learn/enfermedades-no-transmisibles) Pontificia Universidad Católica de Chile
* [Clinical Terminology for International and U.S. Students](https://www.coursera.org/learn/clinical-terminology) University of Pittsburgh
* [Diálisis peritoneal](https://www.coursera.org/learn/dialisis-peritoneal) Universidad Nacional Autónoma de México
* [Manejo moderno de la caries dental](https://www.coursera.org/learn/tratamiento-caries) Universidad Nacional Autónoma de México
* [Bacteria and Chronic Infections](https://www.coursera.org/learn/bacterial-infections) University of Copenhagen
* [Essentials in Clinical Simulations Across the Health Professions](https://www.coursera.org/learn/clinicalsimulations) The George Washington University
* [Farmacovigilancia ocular](https://www.coursera.org/learn/farmacovigilancia-ocular) Universidad Nacional Autónoma de México
* [Health Concepts in Chinese Medicine](https://www.coursera.org/learn/health-concepts-chinese-medicine) The Hong Kong University of Science and Technology
* [Case Studies in Personalized Medicine](https://www.coursera.org/learn/personalizedmed) Vanderbilt University
* [Career 911: Your Future Job in Medicine and Healthcare](https://www.coursera.org/learn/healthcarejobs) Northwestern University
* [Clinical Kidney, Pancreas and Islet Transplantation](https://www.coursera.org/learn/clinical-kidney-transplantation) Universiteit Leiden
* [The Basics of Trauma Surgery](https://www.coursera.org/learn/trauma-surgery-basics) Technische Universität München (TUM)
* [Acute and Chronic Rhinosinusitis: A Comprehensive Review](https://www.coursera.org/learn/icahn-school-of-medicine-at-mount-sinai-acute-and-chronic-rhinosinusitis) Icahn School of Medicine at Mount Sinai
* [Introduction to Cataract Surgery](https://www.coursera.org/learn/cataract-surgery) University of Michigan
* [Anticoncepción hormonal al alcance de todos](https://www.coursera.org/learn/anticonconcepcion-hormonal) Universitat Autònoma de Barcelona
* [Репродуктивное здоровье женщины и безопасная беременность](https://www.coursera.org/learn/reproduktivnoe-zdorove-zhenshchiny) National Research Tomsk State University
* [Cáncer de próstata](https://www.coursera.org/learn/cancer-prostata) Universidad Nacional Autónoma de México
* [Teaching and Assessing Clinical Skills](https://www.coursera.org/learn/clinical-skills) University of Michigan
* [Atención prehospitalaria del ictus agudo y selección de pacientes para tratamiento endovascular con la escala RACE](https://www.coursera.org/learn/ictus-agudo-escala-race) Universitat de Barcelona
* [Introduction to Hearing Loss](https://www.coursera.org/learn/hearing-loss) Icahn School of Medicine at Mount Sinai
* [Foundations for Assisting in Home Care](https://www.coursera.org/learn/home-care) The State University of New York
* [AIDS: Fear and Hope](https://www.coursera.org/learn/aids-fear-hope) University of Michigan
* [Grundlagen der Unfallchirurgie](https://www.coursera.org/learn/unfallchirurgie) Technische Universität München (TUM)
* [Ebola: Essential Knowledge for Health Professionals](https://www.coursera.org/learn/ebola-essentials-for-health-professionals) University of Amsterdam
* [PrEParing: PrEP for Providers and Patients](https://www.coursera.org/learn/prep) Johns Hopkins University
* [杏林探宝——认知中药](https://www.coursera.org/learn/zhong-yao-zhi-shi) Shanghai Jiao Tong University
* [口腔种植学 （Implant Dentistry）](https://www.coursera.org/learn/implant-dentistry-chinese) The University of Hong Kong
* [Prehospital care of acute stroke and patient selection for endovascular treatment using the RACE scale](https://www.coursera.org/learn/acute-stroke-race-scale) Universitat de Barcelona
* [Supervision du raisonnement clinique](https://www.coursera.org/learn/supervision-raisonnement-clinique) University of Geneva
* [一堂課讓你認識肺癌（Basic Concepts of Lung Cancer: Diagnosis and Treatment）](https://www.coursera.org/learn/lung-cancer) National Taiwan University
* [Population Health: Panel Management Next Level](https://www.coursera.org/learn/panel-management) Universiteit Leiden
* [İnfertilite Hemşireliği (Infertility Nursing)](https://www.coursera.org/learn/infertilite) Koç University
* [常见慢性病的健康管理](https://www.coursera.org/learn/chang-jian-man-xing-bing) Shanghai Jiao Tong University
* [ÉCHELLE RACE: Dépistage préhospitalier de l’AVC impliquant une occlusion de gros vaisseaux cérébraux](https://www.coursera.org/learn/prestorace-fr) Universitat de Barcelona
* [更年期综合管理](https://www.coursera.org/learn/geng-nian-qi) Peking University


## life-sciences/psychology

* [Introduction to Psychology](https://www.coursera.org/learn/introduction-psychology) Yale University
* [Primeros Auxilios Psicológicos (PAP)](https://www.coursera.org/learn/pap) Universitat Autònoma de Barcelona
* [Buddhism and Modern Psychology](https://www.coursera.org/learn/science-of-meditation) Princeton University
* [Psychological First Aid](https://www.coursera.org/learn/psychological-first-aid) Johns Hopkins University
* [Introduction to Psychology](https://www.coursera.org/learn/introduction-psych) University of Toronto
* [Moralities of Everyday Life](https://www.coursera.org/learn/moralities) Yale University
* [Mind Control: Managing Your Mental Health During COVID-19](https://www.coursera.org/learn/manage-health-covid-19) University of Toronto
* [Sexualidad...mucho más que sexo](https://www.coursera.org/learn/sexualidad) Universidad de los Andes
* [Introduction to User Experience Design](https://www.coursera.org/learn/user-experience-design) Georgia Institute of Technology
* [An Introduction to Consumer Neuroscience & Neuromarketing](https://www.coursera.org/learn/neuromarketing) Copenhagen Business School
* [Addiction Treatment: Clinical Skills for Healthcare Providers](https://www.coursera.org/learn/addiction-treatment) Yale University
* [Children's Human Rights - An Interdisciplinary Introduction](https://www.coursera.org/learn/childrens-rights) University of Geneva
* [Improving your statistical inferences](https://www.coursera.org/learn/statistical-inferences) Eindhoven University of Technology
* [Troubles du spectre de l'autisme : diagnostic](https://www.coursera.org/learn/troubles-spectre-autisme-diagnostic) University of Geneva
* [Primeros Auxilios Psicológicos (PAP). Edición especial COVID-19](https://www.coursera.org/learn/pap-covid19) Universitat Autònoma de Barcelona
* [Schizophrenia](https://www.coursera.org/learn/schizophrenia) Wesleyan University
* [Речевой этикет: вежливость и коммуникативные стратегии](https://www.coursera.org/learn/rechevoj-etiket) National Research University Higher School of Economics
* [Управление человеческими ресурсами](https://www.coursera.org/learn/upravleniye-chelovecheskimi-resursami) Peter the Great St. Petersburg Polytechnic University
* [The Bilingual Brain](https://www.coursera.org/learn/bilingual) University of Houston System
* [Introduction to Human Behavioral Genetics](https://www.coursera.org/learn/behavioralgenetics) University of Minnesota
* [Actúa ante el dolor crónico](https://www.coursera.org/learn/actua-dolor-cronico) Universitat Autònoma de Barcelona
* [How Music Can Change Your Life](https://www.coursera.org/learn/music-life) The University of Melbourne
* [Tu consultorio de Coaching en las ondas](https://www.coursera.org/learn/coaching-en-las-ondas) Universitat Autònoma de Barcelona
* [Зоопсихология](https://www.coursera.org/learn/zoopsikhologiya) National Research Tomsk State University
* [Психология межгрупповых отношений](https://www.coursera.org/learn/psikhologiya-mejgruppovykh-otnoshenii) National Research University Higher School of Economics
* [Unethical Decision Making in Organizations](https://www.coursera.org/learn/unethical-decision-making) University of Lausanne
* [Статистические методы в гуманитарных исследованиях](https://www.coursera.org/learn/statistics-for-humanities) National Research Tomsk State University
* [מבוא למדעי הפסיכולוגיה - Introduction to Psychological Science](https://www.coursera.org/learn/psychology-science-intro) Tel Aviv University
* [心理学与生活](https://www.coursera.org/learn/xin-li-xue-sheng-huo) Nanjing University
* [發展心理學：哲學觀與方法論 (Developmental Psychology: Philosophical Bases and Methodology)](https://www.coursera.org/learn/developmental-psychology) National Taiwan University
* [当代应用心理学](https://www.coursera.org/learn/dangdai-yingyong-xinli-xue) Shanghai Jiao Tong University
* [Dopage : Sports, Organisations et Sciences](https://www.coursera.org/learn/dopage) University of Lausanne
* [Soul Beliefs: Causes and Consequences - Unit 3: How Does It All End?](https://www.coursera.org/learn/soulbeliefs3) Rutgers the State University of New Jersey


## life-sciences/public-health

* [Science Matters: Let's Talk About COVID-19](https://www.coursera.org/learn/covid-19) Imperial College London
* [Fighting COVID-19 with Epidemiology: A Johns Hopkins Teach-Out](https://www.coursera.org/learn/covid19-epidemiology) Johns Hopkins University
* [Revisão Sistemática e Meta-análise](https://www.coursera.org/learn/revisao-sistematica) Universidade Estadual de Campinas
* [Epidemiology: The Basic Science of Public Health](https://www.coursera.org/learn/epidemiology) The University of North Carolina at Chapel Hill
* [COVID-19: What You Need to Know (CME Eligible)](https://www.coursera.org/learn/covid-19-what-you-need-to-know) Osmosis
* [Cuidados y procedimientos generales en la atención del recién nacido](https://www.coursera.org/learn/cuidados-del-recien-nacido) Universidad de Chile
* [International Women's Health and Human Rights](https://www.coursera.org/learn/womens-health-human-rights) Stanford University
* [Essentials of Global Health](https://www.coursera.org/learn/essentials-global-health) Yale University
* [Stories of Infection](https://www.coursera.org/learn/stories-of-infection) Stanford University
* [Dermatology: Trip to skin](https://www.coursera.org/learn/dermatology) Novosibirsk State University
* [Antibiotic Stewardship](https://www.coursera.org/learn/antibiotic-stewardship) Stanford University
* [Evaluación del Aprendizaje en Escenarios Clínicos](https://www.coursera.org/learn/evaluacion-aprendizaje-escenarios-clinicos) Tecnológico de Monterrey
* [Health Across the Gender Spectrum](https://www.coursera.org/learn/health-gender-spectrum) Stanford University
* [The Challenges of Global Health](https://www.coursera.org/learn/global-health) Duke University
* [Resilience in Children Exposed to Trauma, Disaster and War: Global Perspectives](https://www.coursera.org/learn/resilience-in-children) University of Minnesota
* [Systems Thinking In Public Health](https://www.coursera.org/learn/systems-thinking) Johns Hopkins University
* [Epidemics](https://www.coursera.org/learn/hkuepidemics) The University of Hong Kong
* [Drugs, drug use, drug policy and health](https://www.coursera.org/learn/drugs) University of Geneva
* [Infection Prevention in Nursing Homes](https://www.coursera.org/learn/infection-prevention) The University of North Carolina at Chapel Hill
* [Major Depression in the Population: A Public Health Approach](https://www.coursera.org/learn/public-health-depression) Johns Hopkins University
* [Disease Screening in Public Health](https://www.coursera.org/learn/screening) University of Geneva
* [Global Health: An Interdisciplinary Overview](https://www.coursera.org/learn/global-health-overview) University of Geneva
* [An Introduction to Global Health](https://www.coursera.org/learn/global-health-introduction) University of Copenhagen
* [Diabetes - a Global Challenge](https://www.coursera.org/learn/diabetes) University of Copenhagen
* [Confronting Gender Based Violence: Global Lessons for Healthcare Workers](https://www.coursera.org/learn/gender-based-violence) Johns Hopkins University
* [La Solución del Conflicto Ético](https://www.coursera.org/learn/etica) Universidad Nacional Autónoma de México
* [Disease Clusters](https://www.coursera.org/learn/disease-clusters) Johns Hopkins University
* [Global Health at the Human-Animal-Ecosystem Interface](https://www.coursera.org/learn/global-health-human-animal-ecosystem) University of Geneva
* [Population Health: Health & Health Behaviour](https://www.coursera.org/learn/population-health-behaviour) Universiteit Leiden
* [Michigan Sport-Related Concussion Training Certification](https://www.coursera.org/learn/michigan-sport-related-concussion-training-certification) University of Michigan
* [Air Pollution – a Global Threat to our Health](https://www.coursera.org/learn/air-pollution-health-threat) University of Copenhagen
* [Diagnóstico y tratamiento del dolor neuropático en atención primaria](https://www.coursera.org/learn/dolor-neuropatico-anestesiologia) Universidad de los Andes
* [Global Health Policy](https://www.coursera.org/learn/global-health-policy) The University of Tokyo
* [Здоровое сердце, здоровые сосуды](https://www.coursera.org/learn/zdorovoe-serdce) National Research Tomsk State University
* [Instructional Methods in Health Professions Education](https://www.coursera.org/learn/instructional-methods-education) University of Michigan
* [Unravelling solutions for Future Food problems](https://www.coursera.org/learn/solutions-future-food-problem) Utrecht University
* [International Travel Preparation, Safety, & Wellness](https://www.coursera.org/learn/international-travel) Johns Hopkins University
* [Global Health Diplomacy](https://www.coursera.org/learn/global-health-diplomacy) The State University of New York
* [An Introduction to the U.S. Food System: Perspectives from Public Health](https://www.coursera.org/learn/food-system) Johns Hopkins University
* [Easing the burden of obesity, diabetes and cardiovascular disease](https://www.coursera.org/learn/easing-the-burden-of-obesity-diabetes-cvd) The University of Sydney
* [Life, Health and Radiation](https://www.coursera.org/learn/life-health-radiation) The University of Sydney
* [Ebola Virus Disease: An Evolving Epidemic](https://www.coursera.org/learn/ebola-virus) Emory University
* [Global Health and Humanitarianism](https://www.coursera.org/learn/health-humanitarianism) University of Manchester
* [Public Health in Humanitarian Crises 2](https://www.coursera.org/learn/humanitarian-public-health-2) Johns Hopkins University
* [Reducing Gun Violence in America: Evidence for Change](https://www.coursera.org/learn/gun-violence) Johns Hopkins University
* [Engineering Life: Synbio, Bioethics & Public Policy](https://www.coursera.org/learn/synbioethics) Johns Hopkins University
* [Global Health Security, Solidarity and Sustainability through the International Health Regulations](https://www.coursera.org/learn/international-health-regulations) University of Geneva
* [Systems Science and Obesity](https://www.coursera.org/learn/systems-science-obesity) Johns Hopkins University
* [Population Health: Study Design](https://www.coursera.org/learn/population-health-study-design) Universiteit Leiden
* [Childbirth: A Global Perspective](https://www.coursera.org/learn/childbirth) Emory University
* [Everyday Chinese Medicine 2](https://www.coursera.org/learn/everyday-chinese-medicine-2) The Chinese University of Hong Kong
* [Identifying Patient Populations](https://www.coursera.org/learn/computational-phenotyping) University of Colorado System
* [Protecting Public Health in a Changing Climate: A Primer for City, Local, and Regional Action](https://www.coursera.org/learn/climate-change) Johns Hopkins University
* [Population Health: Governance](https://www.coursera.org/learn/population-health-governance) Universiteit Leiden
* [Non-Communicable Diseases in Humanitarian Settings](https://www.coursera.org/learn/non-communicable-diseases-in-humanitarian-settings) University of Copenhagen
* [中医药与中华传统文化](https://www.coursera.org/learn/zhong-yi-yao-wen-hua) Shanghai Jiao Tong University
* [The People, Power, and Pride of Public Health](https://www.coursera.org/learn/public-health) Johns Hopkins University
* [Foundations of Health Equity Research](https://www.coursera.org/learn/health-equity-research) Johns Hopkins University
* [Health and healthcare in transition: dilemmas of governance](https://www.coursera.org/learn/health-dilemmas-of-governance) National Research Tomsk State University
* [Ebola : Vaincre ensemble !](https://www.coursera.org/learn/ebola-vaincre-ensemble) University of Geneva
* [Foundations for Global Health Responders](https://www.coursera.org/learn/ghresponder) University of Colorado System


## life-sciences/research

* [Medical Neuroscience](https://www.coursera.org/learn/medical-neuroscience) Duke University
* [Understanding Clinical Research: Behind the Statistics](https://www.coursera.org/learn/clinical-research) University of Cape Town
* [Introduction to Systematic Review and Meta-Analysis](https://www.coursera.org/learn/systematic-review) Johns Hopkins University
* [Design and Interpretation of Clinical Trials](https://www.coursera.org/learn/clinical-trials) Johns Hopkins University
* [Data Management for Clinical Research](https://www.coursera.org/learn/clinical-data-management) Vanderbilt University
* [Whole genome sequencing of bacterial genomes - tools and applications](https://www.coursera.org/learn/wgs-bacteria) Technical University of Denmark (DTU)
* [Getting started in cryo-EM](https://www.coursera.org/learn/cryo-em) Caltech
* [MRI Fundamentals](https://www.coursera.org/learn/mri-fundamentals) Korea Advanced Institute of Science and Technology(KAIST)
* [Medical Applications of Particle Accelerators (NPAP MOOC)](https://www.coursera.org/learn/medical-applications-particle-accelerators) Lund University
* [Power and Sample Size for Multilevel and Longitudinal Study Designs](https://www.coursera.org/learn/power-sample-size) University of Florida
* [Биосенсоры](https://www.coursera.org/learn/biosensory) Novosibirsk State University
* [Doing Clinical Research: Biostatistics with the Wolfram Language](https://www.coursera.org/learn/clinical-research-biostatistics-wolfram) University of Cape Town


## math-and-logic/math-and-logic

* [Game Theory](https://www.coursera.org/learn/game-theory-1) Stanford University
* [Álgebra Básica](https://www.coursera.org/learn/algebra-basica) Universidad Nacional Autónoma de México
* [Data Science Math Skills](https://www.coursera.org/learn/datasciencemathskills) Duke University
* [Introduction to Calculus](https://www.coursera.org/learn/introduction-to-calculus) The University of Sydney
* [Calculus: Single Variable Part 1 - Functions](https://www.coursera.org/learn/single-variable-calculus) University of Pennsylvania
* [Cryptography I](https://www.coursera.org/learn/crypto) Stanford University
* [Estadística y probabilidad](https://www.coursera.org/learn/estadistica-probabilidad) Universidad Nacional Autónoma de México
* [Bayesian Statistics: From Concept to Data Analysis](https://www.coursera.org/learn/bayesian-statistics) University of California, Santa Cruz
* [Probability and Statistics: To p or not to p?](https://www.coursera.org/learn/probability-statistics) University of London
* [Econometrics: Methods and Applications](https://www.coursera.org/learn/erasmus-econometrics) Erasmus University Rotterdam
* [Machine Design Part I](https://www.coursera.org/learn/machine-design1) Georgia Institute of Technology
* [Cálculo Diferencial e Integral unidos por el Teorema Fundamental del Cálculo](https://www.coursera.org/learn/calculo-diferencial) Tecnológico de Monterrey
* [Pre-Calculus](https://www.coursera.org/learn/introduccion-al-calculo) Universitat Autònoma de Barcelona
* [Practical Time Series Analysis](https://www.coursera.org/learn/practical-time-series-analysis) The State University of New York
* [Matrix Algebra for Engineers](https://www.coursera.org/learn/matrix-algebra-engineers) The Hong Kong University of Science and Technology
* [Эконометрика (Econometrics)](https://www.coursera.org/learn/ekonometrika) National Research University Higher School of Economics
* [Discrete Optimization](https://www.coursera.org/learn/discrete-optimization) The University of Melbourne
* [1.- El Cálculo - Modelo Lineal](https://www.coursera.org/learn/calculo-1) Tecnológico de Monterrey
* [Differential Equations for Engineers](https://www.coursera.org/learn/differential-equations-engineers) The Hong Kong University of Science and Technology
* [Теория игр (Game Theory)](https://www.coursera.org/learn/game-theory) National Research University Higher School of Economics
* [Introduction to Ordinary Differential Equations](https://www.coursera.org/learn/ordinary-differential-equations) Korea Advanced Institute of Science and Technology(KAIST)
* [Линейная алгебра (Linear Algebra)](https://www.coursera.org/learn/algebra-lineynaya) National Research University Higher School of Economics
* [Física: Vectores, Trabajo y Energía](https://www.coursera.org/learn/fisica-vectores-trabajo-energia) Tecnológico de Monterrey
* [Introduction to Complex Analysis](https://www.coursera.org/learn/complex-analysis) Wesleyan University
* [Vector Calculus for Engineers](https://www.coursera.org/learn/vector-calculus-engineers) The Hong Kong University of Science and Technology
* [Introduction into General Theory of Relativity](https://www.coursera.org/learn/general-relativity) National Research University Higher School of Economics
* [Calculus: Single Variable Part 2 - Differentiation](https://www.coursera.org/learn/differentiation-calculus) University of Pennsylvania
* [Mathematical Biostatistics Boot Camp 1](https://www.coursera.org/learn/biostatistics) Johns Hopkins University
* [Interest Rate Models](https://www.coursera.org/learn/interest-rate-models) École Polytechnique Fédérale de Lausanne
* [Electrodynamics: An Introduction](https://www.coursera.org/learn/electrodynamics-introduction) Korea Advanced Institute of Science and Technology(KAIST)
* [Conceptos y Herramientas para la Física Universitaria](https://www.coursera.org/learn/fisica-universitaria) Tecnológico de Monterrey
* [Calculus: Single Variable Part 3 - Integration](https://www.coursera.org/learn/integration-calculus) University of Pennsylvania
* [Física: Dimensión y Movimiento](https://www.coursera.org/learn/fisica-dimension-movimiento) Tecnológico de Monterrey
* [Fibonacci Numbers and the Golden Ratio](https://www.coursera.org/learn/fibonacci) The Hong Kong University of Science and Technology
* [Enjoyable Econometrics](https://www.coursera.org/learn/enjoyable-econometrics) Erasmus University Rotterdam
* [Single Variable Calculus](https://www.coursera.org/learn/discrete-calculus) University of Pennsylvania
* [Information Theory](https://www.coursera.org/learn/information-theory) The Chinese University of Hong Kong
* [Discrete Mathematics](https://www.coursera.org/learn/discrete-mathematics) Shanghai Jiao Tong University
* [Mechanics of Materials III: Beam Bending](https://www.coursera.org/learn/beam-bending) Georgia Institute of Technology
* [Физика в опытах. Часть 1. Механика](https://www.coursera.org/learn/fizika-v-opitah-mehanika) National Research Nuclear University MEPhI
* [Causal Inference](https://www.coursera.org/learn/causal-inference) Columbia University
* [Game Theory II: Advanced Applications](https://www.coursera.org/learn/game-theory-2) Stanford University
* [Линейная алгебра и аналитическая геометрия](https://www.coursera.org/learn/lineynaya-algebra) Peter the Great St. Petersburg Polytechnic University
* [Introduction to Galois Theory](https://www.coursera.org/learn/galois) National Research University Higher School of Economics
* [Logic for Economists](https://www.coursera.org/learn/logic-for-economists) University of Amsterdam
* [离散数学概论 Discrete Mathematics Generality](https://www.coursera.org/learn/dmathgen) Peking University
* [Introducción al análisis de Costos para la Dirección de Empresas](https://www.coursera.org/learn/analisis-costos-direccion-empresas) Universidad Austral
* [頑想學概率：機率一 (Probability (1))](https://www.coursera.org/learn/prob1) National Taiwan University
* [Calculus: Single Variable Part 4 - Applications](https://www.coursera.org/learn/applications-calculus) University of Pennsylvania
* [Analytic Combinatorics](https://www.coursera.org/learn/analytic-combinatorics) Princeton University
* [Алгоритмизация вычислений (Algorithmic computation)](https://www.coursera.org/learn/algoritmizacija-vychislenij) National Research University Higher School of Economics
* [Electrodynamics: Electric and Magnetic Fields](https://www.coursera.org/learn/electrodynamics-electric-magnetic-fields) Korea Advanced Institute of Science and Technology(KAIST)
* [Introduction to Enumerative Combinatorics](https://www.coursera.org/learn/enumerative-combinatorics) National Research University Higher School of Economics
* [Физика в опытах. Часть 2. Электричество и магнетизм](https://www.coursera.org/learn/fizika-v-opitah-elektrichestvo-i-magnetizm) National Research Nuclear University MEPhI
* [2.- El Cálculo - Modelo Cuadrático](https://www.coursera.org/learn/calculo-2) Tecnológico de Monterrey
* [Analyse numérique pour ingénieurs](https://www.coursera.org/learn/analyse-numerique) École Polytechnique Fédérale de Lausanne
* [Введение в математические методы физики](https://www.coursera.org/learn/vvedenie-v-mat-metody) National Research University Higher School of Economics
* [Advanced Linear Models for Data Science 1: Least Squares](https://www.coursera.org/learn/linear-models) Johns Hopkins University
* [Electrodynamics: In-depth Solutions for Maxwell’s Equations](https://www.coursera.org/learn/electrodynamics-solutions-maxwells-equations) Korea Advanced Institute of Science and Technology(KAIST)
* [Matrix Methods](https://www.coursera.org/learn/matrix-methods) University of Minnesota
* [Electrodynamics: Analysis of Electric Fields](https://www.coursera.org/learn/electrodynamics-analysis-of-electric-fields) Korea Advanced Institute of Science and Technology(KAIST)
* [Introduction à la théorie de Galois](https://www.coursera.org/learn/theorie-de-galois) École normale supérieure
* [Применение производной и интеграла в курсе общей физики](https://www.coursera.org/learn/proizvodnaya-i-integral-v-fizike) National Research Nuclear University MEPhI
* [3.- El Cálculo - Modelo Cúbico](https://www.coursera.org/learn/calculo-3) Tecnológico de Monterrey
* [竞争策略（中文版）](https://www.coursera.org/learn/competitivestrategyzh) Ludwig-Maximilians-Universität München (LMU)
* [Introduction to Formal Concept Analysis](https://www.coursera.org/learn/formal-concept-analysis) National Research University Higher School of Economics
* [Games without Chance: Combinatorial Game Theory](https://www.coursera.org/learn/combinatorial-game-theory) Georgia Institute of Technology
* [Invitation to Mathematics הזמנה למתמטיקה](https://www.coursera.org/learn/introduction-to-math) Hebrew University of Jerusalem
* [Mathematical Biostatistics Boot Camp 2](https://www.coursera.org/learn/biostatistics-2) Johns Hopkins University
* [Advanced Linear Models for Data Science 2: Statistical Linear Models](https://www.coursera.org/learn/linear-models-2) Johns Hopkins University
* [Çok değişkenli Fonksiyon I: Kavramlar / Multivariable Calculus I: Concepts](https://www.coursera.org/learn/hesap-calculus-dersi) Koç University
* [頑想學概率：機率二 (Probability (2))](https://www.coursera.org/learn/prob2) National Taiwan University
* [离散数学](https://www.coursera.org/learn/discrete-mathematics-ch) Shanghai Jiao Tong University
* [Introduzione alla fisica sperimentale: meccanica, termodinamica](https://www.coursera.org/learn/fisica-sperimentale-meccanica-termodinamica) Politecnico di Milano
* [Causal Inference 2](https://www.coursera.org/learn/causal-inference-2) Columbia University
* [4.- El Cálculo - Otros Modelos](https://www.coursera.org/learn/calculo-4) Tecnológico de Monterrey
* [Doğrusal Cebir I: Uzaylar ve İşlemciler / Linear Algebra I: Spaces and Operators](https://www.coursera.org/learn/linearalgebra1) Koç University
* [Jacobi modular forms: 30 ans après](https://www.coursera.org/learn/modular-forms-jacobi) National Research University Higher School of Economics
* [Mécanique Lagrangienne](https://www.coursera.org/learn/mecanique-lagrangienne) École Polytechnique Fédérale de Lausanne
* [Aléatoire : une introduction aux probabilités - Partie 2](https://www.coursera.org/learn/probabilites-2) École Polytechnique


## personal-development/personal-development

* [The Science of Well-Being](https://www.coursera.org/learn/the-science-of-well-being) Yale University
* [Learning How to Learn: Powerful mental tools to help you master tough subjects](https://www.coursera.org/learn/learning-how-to-learn) McMaster University
* [Successful Negotiation: Essential Strategies and Skills](https://www.coursera.org/learn/negotiation-skills) University of Michigan
* [Social Psychology](https://www.coursera.org/learn/social-psychology) Wesleyan University
* [Mindshift: Break Through Obstacles to Learning and Discover Your Hidden Potential](https://www.coursera.org/learn/mindshift) McMaster University
* [Aprendiendo a aprender: Poderosas herramientas mentales con las que podrás dominar temas difíciles (Learning How to Learn)](https://www.coursera.org/learn/aprendiendo-a-aprender) McMaster University
* [A Life of Happiness and Fulfillment](https://www.coursera.org/learn/happiness) Indian School of Business
* [Writing in the Sciences](https://www.coursera.org/learn/sciwrite) Stanford University
* [Competencias digitales. Herramientas de ofimática (Microsoft Word, Excel, Power Point)](https://www.coursera.org/learn/competencias-digitales-ofimatica) Universitat Autònoma de Barcelona
* [Introduction to Mathematical Thinking](https://www.coursera.org/learn/mathematical-thinking) Stanford University
* [Think Again I: How to Understand Arguments](https://www.coursera.org/learn/understanding-arguments) Duke University
* [Aprender](https://www.coursera.org/learn/aprendo) Universidad Nacional Autónoma de México
* [Fundamentals of Music Theory](https://www.coursera.org/learn/edinburgh-music-theory) The University of Edinburgh
* [Introduction to Personal Branding](https://www.coursera.org/learn/personal-branding) University of Virginia
* [Cómo hablar bien en público](https://www.coursera.org/learn/hablar-bien-en-publico) Universitat Autònoma de Barcelona
* [Learning to Teach Online](https://www.coursera.org/learn/teach-online) UNSW Sydney (The University of New South Wales)
* [De-Mystifying Mindfulness](https://www.coursera.org/learn/mindfulness) Universiteit Leiden
* [The Arts and Science of Relationships: Understanding Human Needs](https://www.coursera.org/learn/human-needs) University of Toronto
* [Creative Thinking: Techniques and Tools for Success](https://www.coursera.org/learn/creative-thinking-techniques-and-tools-for-success) Imperial College London
* [Everyday Parenting: The ABCs of Child Rearing](https://www.coursera.org/learn/everyday-parenting) Yale University
* [¿Cómo persuadir? Jugando con palabras, imágenes y números](https://www.coursera.org/learn/como-persuadir) Universitat Autònoma de Barcelona
* [Negociación exitosa: Estrategias y habilidades esenciales (en español)](https://www.coursera.org/learn/negociacion) University of Michigan
* [Основы фотографии](https://www.coursera.org/learn/photo) Novosibirsk State University
* [Introducción a la Producción Audiovisual](https://www.coursera.org/learn/intro-produccion-audiovisual) Universidad Nacional Autónoma de México
* [The Manager's Toolkit: A Practical Guide to Managing People at Work](https://www.coursera.org/learn/people-management) University of London
* [Meditation: A way to achieve your goals in your life](https://www.coursera.org/learn/self-reflection-meditation) Korea Advanced Institute of Science and Technology(KAIST)
* [Becoming a changemaker: Introduction to Social Innovation](https://www.coursera.org/learn/social-innovation) University of Cape Town
* [Основы поиска дела жизни. Часть 1. Как перестать откладывать дела на потом?](https://www.coursera.org/learn/prednaznachenie-delo-jizni) National Research Nuclear University MEPhI
* [Aprendendo a aprender: ferramentas mentais poderosas para ajudá-lo a dominar assuntos difíceis (em Português) [Learning How to Learn]](https://www.coursera.org/learn/aprender) McMaster University
* [English for Media Literacy](https://www.coursera.org/learn/media) University of Pennsylvania
* [Potenciando mi aprendizaje en el primer año de Universidad](https://www.coursera.org/learn/potenciando-aprendizaje) Universidad de Chile
* [Sit Less, Get Active](https://www.coursera.org/learn/get-active) The University of Edinburgh
* [Теория Лжи. Профайлинг](https://www.coursera.org/learn/teoriya-lzhi-profajling) National Research Tomsk State University
* [Bienestar, equidad y derechos humanos](https://www.coursera.org/learn/bienestar-equidad-derechos-humanos) Universidad de los Andes
* [Учимся учиться. Как преуспеть в школе, не тратя всё время на учёбу](https://www.coursera.org/learn/learnhow) National Research University Higher School of Economics
* [تعّلم كيف تتعلم: أدوات ذهنية قوية لمساعدتك على إتقان موضوعات صعبة](https://www.coursera.org/learn/learning-how-to-learn-ar) McMaster University
* [Pensamiento Sistémico](https://www.coursera.org/learn/pensamiento-sistemico) Universidad Nacional Autónoma de México
* [Stanford's Short Course on Breastfeeding](https://www.coursera.org/learn/breastfeeding) Stanford University
* [Devenir entrepreneur du changement](https://www.coursera.org/learn/entrepreneur-changement) HEC Paris
* [Successful Career Development](https://www.coursera.org/learn/career-advancement) University System of Georgia
* [Learning How To Learn for Youth](https://www.coursera.org/learn/learning-how-to-learn-youth) Arizona State University
* [English for Teaching Purposes](https://www.coursera.org/learn/teaching-english) Universitat Autònoma de Barcelona
* [Gut Check: Exploring Your Microbiome](https://www.coursera.org/learn/microbiome) University of Colorado Boulder
* [Understanding Memory: Explaining the Psychology of Memory through Movies](https://www.coursera.org/learn/memory-and-movies) Wesleyan University
* [Negociación 4.0](https://www.coursera.org/learn/negociacion-iae) Universidad Austral
* [ADHD: Everyday Strategies for Elementary Students](https://www.coursera.org/learn/adhd-treatment) The State University of New York
* [Leadership in 21st Century Organizations](https://www.coursera.org/learn/leadership-21st-century) Copenhagen Business School
* [Know Thyself - The Value and Limits of Self-Knowledge: The Examined Life](https://www.coursera.org/learn/know-thyself-the-examined-life) The University of Edinburgh
* [How to Get Skilled: Introduction to Individual Skills Management (Project-Centered Course)](https://www.coursera.org/learn/skills-management) The State University of New York
* [Competencias digitales. Bases de datos: Access](https://www.coursera.org/learn/competencias-digitales-access) Universitat Autònoma de Barcelona
* [Know Thyself - The Value and Limits of Self-Knowledge: The Unconscious](https://www.coursera.org/learn/know-thyself-the-unconscious) The University of Edinburgh
* [Практика разрешения конфликтов. Я - семья - работа - общество](https://www.coursera.org/learn/conflict-resolution) National Research Tomsk State University
* [Managing Your Health: The Role of Physical Therapy and Exercise](https://www.coursera.org/learn/physical-therapy-exercise) University of Toronto
* [Renewable Energy and Green Building Entrepreneurship](https://www.coursera.org/learn/renewable-energy-entrepreneurship) Duke University
* [Applying to U.S. Universities](https://www.coursera.org/learn/study-in-usa) University of Pennsylvania
* [Sleep: Neurobiology, Medicine, and Society](https://www.coursera.org/learn/sleep) University of Michigan
* [Mindware: Critical Thinking for the Information Age](https://www.coursera.org/learn/mindware) University of Michigan
* [An Intuitive Introduction to Probability](https://www.coursera.org/learn/introductiontoprobability) University of Zurich
* [Réussir le Changement](https://www.coursera.org/learn/reussir-le-changement) ESSEC Business School
* [Negociações de sucesso: estratégias e habilidades essenciais (em Português)](https://www.coursera.org/learn/negociacao) University of Michigan
* [Exploring Emerging Technologies for Lifelong Learning and Success](https://www.coursera.org/learn/emerging-technologies-lifelong-learning) The State University of New York
* [Contenido de las matemáticas de primaria](https://www.coursera.org/learn/contenido-matematica-escolar) Universidad de los Andes
* [Apprendre comment apprendre (ACA) : Des outils mentaux puissants qui vous aideront à maîtriser des sujets difficiles](https://www.coursera.org/learn/apprendre-comment-apprendre) McMaster University
* [How to Apply to College](https://www.coursera.org/learn/applying-to-college) University of Pennsylvania
* [Oceanografía: una clave para entender mejor nuestro mundo](https://www.coursera.org/learn/oceanografia) Universitat de Barcelona
* [The Science of Training Young Athletes](https://www.coursera.org/learn/youth-sports) University of Florida
* [Liderazgo Instruccional: Perspectiva Global y Prácticas Locales](https://www.coursera.org/learn/liderazgo-educativo) Pontificia Universidad Católica de Chile
* [Ignite Your Everyday Creativity](https://www.coursera.org/learn/ignite-creativity) The State University of New York
* [Introducción al Aprendizaje Universitario](https://www.coursera.org/learn/aprendizaje-universitario-introduccion) Pontificia Universidad Católica de Chile
* [Foundations of Teaching for Learning: Being a Teacher](https://www.coursera.org/learn/being-a-teacher) Commonwealth Education Trust
* [学会如何学习：帮助你掌握复杂学科的强大智力工具（Learning How to Learn）](https://www.coursera.org/learn/ruhe-xuexi) McMaster University
* [Trabajar para ser feliz](https://www.coursera.org/learn/familia-trabajo-sociedad) Universidad Austral
* [Le Bien, le Juste, l'Utile. Introduction aux éthiques philosophiques](https://www.coursera.org/learn/ethique) University of Geneva
* [Gender and Sexuality: Diversity and Inclusion in the Workplace](https://www.coursera.org/learn/gender-sexuality) University of Pittsburgh
* [Formadores de Ciudadanía](https://www.coursera.org/learn/formadores-ciudadania) Universidad de los Andes
* [Job Success: Get Hired or Promoted in 3 Steps](https://www.coursera.org/learn/get-hired) The State University of New York
* [Conflict Transformation](https://www.coursera.org/learn/conflict-transformation) Emory University
* [Учимся понимать ребёнка: руководство для взрослых](https://www.coursera.org/learn/ponimat-rebenka) Novosibirsk State University
* [Studying at Japanese Universities](https://www.coursera.org/learn/study-in-japan) The University of Tokyo
* [Этикет на все случаи жизни](https://www.coursera.org/learn/etiket) National Research Tomsk State University
* [Driving business towards the Sustainable Development Goals](https://www.coursera.org/learn/sdgbusiness) Erasmus University Rotterdam
* [A tanulás tanulása: Hatékony mentális eszközök, melyek segítenek megbirkózni a nehéz tantárgyakkal (Learning How to Learn)](https://www.coursera.org/learn/a-tanulas-tanulasa) McMaster University
* [Resilience Skills in a Time of Uncertainty](https://www.coursera.org/learn/resilience-uncertainty) University of Pennsylvania
* [Voices of Social Change](https://www.coursera.org/learn/voicesofsocialchange) Laureate Education
* [Preventing Chronic Pain: A Human Systems Approach](https://www.coursera.org/learn/chronic-pain) University of Minnesota
* [Foundations of Teaching for Learning: Introduction](https://www.coursera.org/learn/teaching) Commonwealth Education Trust
* [El desafío de Innovar en la Educación Superior](https://www.coursera.org/learn/educacion-superior) Universidad de Chile
* [Etkili Konuşma (Effective Speaking)](https://www.coursera.org/learn/etkili-konusma) Koç University
* [PlanU: escoge la mejor carrera y universidad para ti](https://www.coursera.org/learn/escoger-carrera-y-universidad) Universidad de los Andes
* [Психология признания и самозанятости](https://www.coursera.org/learn/psihologiya-priznaniya-i-samozanyatosti) National Research Tomsk State University
* [Aprendizaje de las matemáticas de primaria](https://www.coursera.org/learn/aprendizaje-matematicas-primaria) Universidad de los Andes
* [Psychodiagnostics and Psychological Assessment](https://www.coursera.org/learn/psychodiagnostics) National Research Tomsk State University
* [Теория и практика создания онлайн-курсов](https://www.coursera.org/learn/howtomooc) Moscow Institute of Physics and Technology
* [Mi Primer Empleo (MPE)](https://www.coursera.org/learn/mi-primer-empleo) Universidad de Chile
* [Competencias digitales. Conceptos y herramientas básicas](https://www.coursera.org/learn/competencias-digitales-herramientas-basicas) Universitat Autònoma de Barcelona
* [Animer une séance collaborative](https://www.coursera.org/learn/animer-seance-collaborative) ESSEC Business School
* [Think Again IV: How to Avoid Fallacies](https://www.coursera.org/learn/logical-fallacies) Duke University
* [Enseñanza de las matemáticas de primaria](https://www.coursera.org/learn/ensenanza-matematicas-primaria) Universidad de los Andes
* [Think Again II: How to Reason Deductively](https://www.coursera.org/learn/deductive-reasoning) Duke University
* [Foundations of Teaching for Learning: Curriculum](https://www.coursera.org/learn/teacher-curriculum) Commonwealth Education Trust
* [Ensino Híbrido: Personalização e Tecnologia na Educação](https://www.coursera.org/learn/ensino-hibrido) Fundação Lemann
* [IBM IT Assessment: Identifying the Right Career for You!](https://www.coursera.org/learn/ibm-it-assessment) IBM
* [Leading for Equity, Diversity and Inclusion in Higher Education](https://www.coursera.org/learn/leading-for-equity-diversity-inclusion) University of Michigan
* [Think Again III: How to Reason Inductively](https://www.coursera.org/learn/inductive-reasoning) Duke University
* [Психология призвания](https://www.coursera.org/learn/psykhologiya-prizvaniya) National Research Tomsk State University
* [Oceanography: a key to better understand our world](https://www.coursera.org/learn/oceanography) Universitat de Barcelona
* [Intellectual Humility: Theory](https://www.coursera.org/learn/intellectual-humility-theory) The University of Edinburgh
* [University Teaching](https://www.coursera.org/learn/university-teaching) The University of Hong Kong
* [Preparing for Graduate Study in the U.S.: A course for international students](https://www.coursera.org/learn/graduate-study-usa) University of Michigan
* [Voces de cambio social](https://www.coursera.org/learn/vocesdecambiosocial) Laureate Education
* [Как найти свою первую работу? Практический курс для студентов вузов](https://www.coursera.org/learn/findjob) National Research University Higher School of Economics
* [Comprender las dimensiones interculturales en la cotidianidad](https://www.coursera.org/learn/interculturalidad) Universidad de los Andes
* [MOOC: How to make a MOOC?](https://www.coursera.org/learn/how-to-mooc) Novosibirsk State University
* [Основы поиска дела жизни. Часть 2. Что скрывается за вопросом "Как найти себя?"](https://www.coursera.org/learn/kak-naiti-sebya) National Research Nuclear University MEPhI
* [Media ethics & governance](https://www.coursera.org/learn/media-ethics-governance) University of Amsterdam
* [Academic Information Seeking](https://www.coursera.org/learn/academicinfoseek) University of Copenhagen
* [Race and Cultural Diversity in American Life and History](https://www.coursera.org/learn/race-cultural-diversity-american-life) University of Illinois at Urbana-Champaign
* [Foundations of Teaching for Learning: Learners and Learning](https://www.coursera.org/learn/teaching-learning) Commonwealth Education Trust
* [Менеджмент профессиональной траектории](https://www.coursera.org/learn/management-proftraektorii) National Research Tomsk State University
* [Здоровье семьи: загадки родословной](https://www.coursera.org/learn/zdorovye-semi-zagadki-rodoslovnoy) National Research Tomsk State University
* [Fundamentos do Google para o Ensino](https://www.coursera.org/learn/fundamentosgoogle) Fundação Lemann
* [القيادة والذكاء العاطفي](https://www.coursera.org/learn/emotional-intelligence-in-leadership-ar) Indian School of Business
* [Digital Footprint](https://www.coursera.org/learn/digital-footprint) The University of Edinburgh
* [ICT in Primary Education: Transforming children's learning across the curriculum](https://www.coursera.org/learn/ict-primary-education) University of London
* [Foundations of Teaching for Learning: Planning for Teaching and Learning](https://www.coursera.org/learn/teaching-plan) Commonwealth Education Trust
* [Understanding Russians: Contexts of Intercultural Communication](https://www.coursera.org/learn/intercultural-communication-russians) National Research University Higher School of Economics
* [Психология труда, инженерная психология и эргономика](https://www.coursera.org/learn/psykhologiya-truda) National Research Tomsk State University
* [Foundations of Teaching for Learning: Introduction to Student Assessment](https://www.coursera.org/learn/learning-assessment) Commonwealth Education Trust
* [Tinkering Fundamentals: Motion and Mechanisms](https://www.coursera.org/learn/tinkering-motion-mechanisms) Exploratorium
* [Skepticism](https://www.coursera.org/learn/skepticism) University of California, Irvine
* [U101: Understanding College and College Life](https://www.coursera.org/learn/college-life) University of Washington
* [How to Change the World](https://www.coursera.org/learn/world-change) Wesleyan University
* [Эксподизайн: проектирование музейной экспозиции в диалогах дизайнера и музеолога](https://www.coursera.org/learn/ekspodizayn) National Research Tomsk State University
* [Tinkering Fundamentals: Circuits](https://www.coursera.org/learn/tinkering-circuits) Exploratorium
* [Educating Deaf Children: Becoming an Empowered Teacher](https://www.coursera.org/learn/educating-deaf-children) University of Cape Town
* [La recherche documentaire](https://www.coursera.org/learn/recherche-documentaire) École Polytechnique
* [الخطابة الإقناعية: تحفيز الجماهير بالحجج المُقنِعة واللغة المؤثِّرة](https://www.coursera.org/learn/persuade-speech-ar) University of Washington
* [Teaching Science at University](https://www.coursera.org/learn/teachingscience) University of Zurich
* [PRINCÍPIOS GERAIS DA TÉCNICA DO VIOLINO E DA VIOLA DE ARCO](https://www.coursera.org/learn/tecnica-violino-viola) Universidade Estadual de Campinas
* [Women in environmental biology](https://www.coursera.org/learn/women-environmental-biology) Universitat Autònoma de Barcelona
* [Intellectual Humility: Practice](https://www.coursera.org/learn/intellectual-humility-practice) The University of Edinburgh
* [Essentials for English Speeches and Presentations 英语演讲与演示](https://www.coursera.org/learn/yingyuyanjiang) Peking University
* [真格—北大在线创业课堂](https://www.coursera.org/learn/zhenge-beida-zaixian-chuangye) Peking University
* [Intellectual Humility: Science](https://www.coursera.org/learn/intellectual-humility-science) The University of Edinburgh
* [Etkili Konuşmada Retorik (Rhetoric in Effective Speaking)](https://www.coursera.org/learn/retorik) Koç University
* [Foundations of Teaching for Learning: Being a Professional](https://www.coursera.org/learn/professional-teacher) Commonwealth Education Trust
* [What does it mean to identify as Transgender or Gender Non-Conforming (TGNC)?](https://www.coursera.org/learn/tgnc-gender-identity-social-change) University of Minnesota
* [Vozes da Mudança Social](https://www.coursera.org/learn/vozes-da-mudanca-social) Laureate Education
* [Teaching Children with Visual Impairment: Creating Empowering Classrooms](https://www.coursera.org/learn/teach-children-with-visual-impairment) University of Cape Town
* [Empowering Yourself in a Post-Truth World](https://www.coursera.org/learn/empowering-yourself-post-truth-world) The State University of New York
* [Genius. Talent. Golden Mediocrity](https://www.coursera.org/learn/genius) National Research Tomsk State University
* [大学生瑜伽](https://www.coursera.org/learn/yoga) Peking University
* [Metaliteracy: Empowering Yourself in a Connected World](https://www.coursera.org/learn/metaliteracy) The State University of New York
* [Professionalism in an era of change](https://www.coursera.org/learn/professionalism-in-an-era-of-change) Utrecht University
* [Создание научно-технического текста](https://www.coursera.org/learn/nauchno-texnicheski-text) National Research Nuclear University MEPhI
* [iMOOC102: Mastering American e-Learning](https://www.coursera.org/learn/e-learning) The State University of New York
* [Journeys to Education Teach-Out](https://www.coursera.org/learn/journeys-to-education-teach-out) Emory University
* [Knowledge Exchange: Using, Protecting and Monetizing Ideas with Third Parties](https://www.coursera.org/learn/knowledge-exchange) Universiteit Leiden
* [Целевые капиталы - территория финансовой стабильности в некоммерческом секторе](https://www.coursera.org/learn/tselevyye-kapitaly) National Research Tomsk State University


## physical-science-and-engineering/chemistry

* [¡¿Cómo?! ¿Química en mi casa?](https://www.coursera.org/learn/quimica-en-mi-casa) Universidad Nacional Autónoma de México
* [Chemistry](https://www.coursera.org/learn/chemistry-1) University of Kentucky
* [Introduction to Chemistry: Reactions and Ratios](https://www.coursera.org/learn/intro-chemistry) Duke University
* [The Science of Gastronomy](https://www.coursera.org/learn/gastronomy) The Hong Kong University of Science and Technology
* [Introduction to Molecular Spectroscopy](https://www.coursera.org/learn/spectroscopy) University of Manchester
* [Nanotechnology and Nanosensors, Part1](https://www.coursera.org/learn/nanotechnology1) Technion - Israel Institute of Technology
* [Chemicals and Health](https://www.coursera.org/learn/chemicals-health) Johns Hopkins University
* [Una aproximación a la Química del Carbono](https://www.coursera.org/learn/qimica-carbono) Universidad Nacional Autónoma de México
* [Advanced Chemistry](https://www.coursera.org/learn/advanced-chemistry) University of Kentucky
* [Introduction to Chemistry: Structures and Solutions](https://www.coursera.org/learn/basic-chemistry) Duke University
* [General Chemistry: Concept Development and Application](https://www.coursera.org/learn/general-chemistry) Rice University
* [Органическая химия](https://www.coursera.org/learn/organicheskaya-khimiya) Novosibirsk State University
* [Exploring Quantum Physics](https://www.coursera.org/learn/quantum-physics) University of Maryland, College Park
* [Неорганическая химия](https://www.coursera.org/learn/neorganicheskayakhimiya) Novosibirsk State University
* [Materials in Oral Health](https://www.coursera.org/learn/materials-oral-health) The University of Hong Kong
* [Физическая химия](https://www.coursera.org/learn/fizicheskaya-khimiya) Novosibirsk State University
* [Organic Solar Cells - Theory and Practice](https://www.coursera.org/learn/solar-cell) Technical University of Denmark (DTU)
* [Materials Data Sciences and Informatics](https://www.coursera.org/learn/material-informatics) Georgia Institute of Technology
* [Introduction to High-Throughput Materials Development](https://www.coursera.org/learn/high-throughput) Georgia Institute of Technology
* [Teaching in University Science Laboratories (Developing Best Practice)](https://www.coursera.org/learn/developing-university-lab-education) University of Amsterdam


## physical-science-and-engineering/electrical-engineering

* [Digital Signal Processing](https://www.coursera.org/learn/dsp) École Polytechnique Fédérale de Lausanne
* [Computer Architecture](https://www.coursera.org/learn/comparch) Princeton University
* [Wind Energy](https://www.coursera.org/learn/wind-energy) Technical University of Denmark (DTU)
* [Electrones en Acción: Electrónica y Arduinos para tus propios Inventos](https://www.coursera.org/learn/electrones-en-accion) Pontificia Universidad Católica de Chile
* [Fundamentals of Digital Image and Video Processing](https://www.coursera.org/learn/digital) Northwestern University
* [Arduino y algunas aplicaciones](https://www.coursera.org/learn/arduino-aplicaciones) Universidad Nacional Autónoma de México
* [Introdução ao Controle de Sistemas](https://www.coursera.org/learn/controle) Instituto Tecnológico de Aeronáutica
* [Digital Systems: From Logic Gates to Processors](https://www.coursera.org/learn/digital-systems) Universitat Autònoma de Barcelona
* [Introduction to TCP/IP](https://www.coursera.org/learn/tcpip) Yonsei University
* [Nanotechnology: A Maker’s Course](https://www.coursera.org/learn/nanotechnology) Duke University
* [Introduction to Systems Engineering](https://www.coursera.org/learn/systems-engineering) UNSW Sydney (The University of New South Wales)
* [Sistemas Digitales: De las puertas lógicas al procesador](https://www.coursera.org/learn/sistemas-digitales) Universitat Autònoma de Barcelona
* [Wireless Communications for Everybody](https://www.coursera.org/learn/wireless-communications) Yonsei University
* [Introduction to Satellite Communications](https://www.coursera.org/learn/satellite-communications) Institut Mines-Télécom
* [Control automático: La tecnología invisible](https://www.coursera.org/learn/control-automatico) Universidad Nacional Autónoma de México
* [Linear Circuits 2: AC Analysis](https://www.coursera.org/learn/linear-circuits-ac-analysis) Georgia Institute of Technology
* [Técnicas Microscópicas de Caracterización](https://www.coursera.org/learn/tecnicas-microscopicas-caracterizacion) Universitat de Barcelona
* [Cómo autoconstruir tu vivienda. Segunda etapa](https://www.coursera.org/learn/como-autoconstruir-tu-vivienda-segunda-etapa) Universidad Nacional Autónoma de México
* [MOS Transistors](https://www.coursera.org/learn/mosfet) Columbia University
* [Silicon Thin Film Solar Cells](https://www.coursera.org/learn/silicon-thin-film-solar-cells) École Polytechnique
* [Controle Usando a Resposta em Frequência](https://www.coursera.org/learn/resposta-frequencia) Instituto Tecnológico de Aeronáutica
* [Ferrous Technology I](https://www.coursera.org/learn/ferrous-technology-1) Pohang University of Science and Technology
* [Comprendre les Microcontroleurs](https://www.coursera.org/learn/microcontroleurs) École Polytechnique Fédérale de Lausanne
* [Plastic electronics](https://www.coursera.org/learn/plastic-electronics) École Polytechnique
* [Averaged-Switch Modeling and Simulation](https://www.coursera.org/learn/averagedswitchmodelingandsimulation) University of Colorado Boulder
* [Recent Advances in Freeform Electronics](https://www.coursera.org/learn/freeform-electronics) Yonsei University
* [Introdução ao Controle Moderno](https://www.coursera.org/learn/controle-moderno) Instituto Tecnológico de Aeronáutica
* [Introduction to Advanced Vibrations](https://www.coursera.org/learn/introduction-advanced-vibrations) Korea Advanced Institute of Science and Technology(KAIST)
* [Ferrous Technology II](https://www.coursera.org/learn/ferrous-technology-2) Pohang University of Science and Technology
* [Fundamentals of particle accelerator technology (NPAP MOOC)](https://www.coursera.org/learn/fundamentals-particle-accelerator-technology) Lund University
* [Enseignes et afficheurs à LED](https://www.coursera.org/learn/enseignes-et-afficheurs-led) École Polytechnique Fédérale de Lausanne
* [Optique non-linéaire](https://www.coursera.org/learn/physique-optique) École Polytechnique
* [Controle de Sistemas no Plano-s](https://www.coursera.org/learn/controle-s) Instituto Tecnológico de Aeronáutica
* [Введение в лазерные технологии](https://www.coursera.org/learn/vveedenie-v-lasernie-tehnologii) National Research Nuclear University MEPhI


## physical-science-and-engineering/environmental-science-and-sustainability

* [English for Science, Technology, Engineering, and Mathematics](https://www.coursera.org/learn/stem) University of Pennsylvania
* [Cómo autoconstruir tu vivienda](https://www.coursera.org/learn/como-autoconstruir-tu-vivienda) Universidad Nacional Autónoma de México
* [Oil & Gas Industry Operations and Markets](https://www.coursera.org/learn/oilandgas) Duke University
* [The Age of Sustainable Development](https://www.coursera.org/learn/sustainable-development) Columbia University
* [Marketing Verde](https://www.coursera.org/learn/marketing-verde) Universidad de los Andes
* [Mountains 101](https://www.coursera.org/learn/mountains-101) University of Alberta
* [Introduction to Thermodynamics: Transferring Energy from Here to There](https://www.coursera.org/learn/thermodynamics-intro) University of Michigan
* [Greening the Economy: Sustainable Cities](https://www.coursera.org/learn/gte-sustainable-cities) Lund University
* [Municipal Solid Waste Management in Developing Countries](https://www.coursera.org/learn/solid-waste-management) École Polytechnique Fédérale de Lausanne
* [Introduction to solar cells](https://www.coursera.org/learn/solar-cells) Technical University of Denmark (DTU)
* [Disaster Preparedness](https://www.coursera.org/learn/disaster-preparedness) University of Pittsburgh
* [Global Environmental Management](https://www.coursera.org/learn/global-environmental-management) Technical University of Denmark (DTU)
* [Circular Economy - Sustainable Materials Management](https://www.coursera.org/learn/circular-economy) Lund University
* [Introduction to Physical Chemistry](https://www.coursera.org/learn/physical-chemistry) University of Manchester
* [Evaluación de peligros y riesgos por fenómenos naturales](https://www.coursera.org/learn/riesgos-fenomenos-naturales) Universidad Nacional Autónoma de México
* [Introducción a la Geotermia](https://www.coursera.org/learn/geotermia) Universidad Nacional Autónoma de México
* [Global Warming I: The Science and Modeling of Climate Change](https://www.coursera.org/learn/global-warming) The University of Chicago
* [Análisis de Sistemas de Transporte](https://www.coursera.org/learn/analisis-sistemas-de-transporte) Pontificia Universidad Católica de Chile
* [Our Earth's Future](https://www.coursera.org/learn/earth-climate-change) American Museum of Natural History
* [Exploring Renewable Energy Schemes](https://www.coursera.org/learn/exploring-renewable-energy) University of Pennsylvania
* [Creativity, Innovation, and Change](https://www.coursera.org/learn/creativity-innovation) The Pennsylvania State University
* [Electric Vehicles and Mobility](https://www.coursera.org/learn/electric-vehicles-mobility) École des Ponts ParisTech
* [Material Behavior](https://www.coursera.org/learn/material-behavior) Georgia Institute of Technology
* [Ecosystem Services: a Method for Sustainable Development](https://www.coursera.org/learn/ecosystem-services) University of Geneva
* [Electric Industry Operations and Markets](https://www.coursera.org/learn/electricity) Duke University
* [Systèmes d’Information Géographique - Partie 1](https://www.coursera.org/learn/sig-1) École Polytechnique Fédérale de Lausanne
* [Introduction to Household Water Treatment and Safe Storage](https://www.coursera.org/learn/water-treatment) École Polytechnique Fédérale de Lausanne
* [Introduction to Algae](https://www.coursera.org/learn/algae) University of California San Diego
* [Sistemas agrosilvopastoriles: una alternativa climáticamente inteligente para la ganadería](https://www.coursera.org/learn/sistemas-agrosilvopastoriles) Universidad Nacional Autónoma de México
* [Conceptos base para el estudio del medio ambiente](https://www.coursera.org/learn/conceptos-estudio-del-medio-ambiente) Universidad Austral
* [Gestión integral del riesgo de desastres](https://www.coursera.org/learn/gestion-riesgo) Universidad Nacional Autónoma de México
* [Las estaciones del año y el clima](https://www.coursera.org/learn/estaciones-clima) Universidad Nacional Autónoma de México
* [Urban Nature: Connecting Cities, Nature and Innovation](https://www.coursera.org/learn/urban-nature) Lund University
* [Sports and Building Aerodynamics](https://www.coursera.org/learn/sports-building-aerodynamics) Eindhoven University of Technology
* [Fundamentals of Fluid-Solid Interactions](https://www.coursera.org/learn/fluid-solid-interaction) École Polytechnique
* [Planning & Design of Sanitation Systems and Technologies](https://www.coursera.org/learn/sanitation) École Polytechnique Fédérale de Lausanne
* [Our Energy Future](https://www.coursera.org/learn/future-of-energy) University of California San Diego
* [Climate Change Mitigation in Developing Countries](https://www.coursera.org/learn/climate-change-mitigation) University of Cape Town
* [Fundamentos de agrotecnología](https://www.coursera.org/learn/fundamentos-agrotecnologia) Universidad Nacional Autónoma de México
* [Sustainable Agricultural Land Management](https://www.coursera.org/learn/sustainable-agriculture) University of Florida
* [Large Marine Ecosystems: Assessment and Management](https://www.coursera.org/learn/large-marine-ecosystems) University of Cape Town
* [Maps and the Geospatial Revolution](https://www.coursera.org/learn/geospatial) The Pennsylvania State University
* [Geographical Information Systems - Part 1](https://www.coursera.org/learn/gis-1) École Polytechnique Fédérale de Lausanne
* [Feeding the World](https://www.coursera.org/learn/feedingtheworld) University of Pennsylvania
* [Fundamentals of Global Energy Business](https://www.coursera.org/learn/energy-business) University of Colorado System
* [Introduction to Environmental Law and Policy](https://www.coursera.org/learn/environmental-law) The University of North Carolina at Chapel Hill
* [Environmental Management & Ethics](https://www.coursera.org/learn/environmental-management-ethics) Technical University of Denmark (DTU)
* [Greening the Economy: Lessons from Scandinavia](https://www.coursera.org/learn/greening-the-economy) Lund University
* [Material Processing](https://www.coursera.org/learn/material-science-engineering) Georgia Institute of Technology
* [Éléments de Géomatique](https://www.coursera.org/learn/geomatique) École Polytechnique Fédérale de Lausanne
* [Wood Science: Beyond Building](https://www.coursera.org/learn/wood-science) West Virginia University
* [Introduction to Indoor Air Quality](https://www.coursera.org/learn/intro-indoor-air-quality) The Hong Kong University of Science and Technology
* [Introducción a los modelos de demanda de transporte](https://www.coursera.org/learn/demanda-de-transporte) Pontificia Universidad Católica de Chile
* [Our Earth: Its Climate, History, and Processes](https://www.coursera.org/learn/our-earth) University of Manchester
* [Les transitions énergétique-écologiques dans les pays du Sud](https://www.coursera.org/learn/transitions-energetiques-pays-du-sud) École normale supérieure
* [Act on Climate: Steps to Individual, Community, and Political Action](https://www.coursera.org/learn/act-on-climate) University of Michigan
* [Green Business Strategy](https://www.coursera.org/learn/green-business-strategy) The Hong Kong University of Science and Technology
* [Comprendre l'écologie, pour une économie innovante](https://www.coursera.org/learn/ecologie) ESCP Business School
* [Sustainability of Social-Ecological Systems: the Nexus between Water, Energy and Food](https://www.coursera.org/learn/sustainability-social-ecological-systems) Universitat Autònoma de Barcelona
* [The Effect of Fires on People, Property and the Environment](https://www.coursera.org/learn/fire-effect) University of Maryland, College Park
* [Introduction to the Arctic: Climate](https://www.coursera.org/learn/arctic-introduction-climate) University of Alberta
* [Introduction to Public Health Engineering in Humanitarian Contexts](https://www.coursera.org/learn/engineering-humanitarian) École Polytechnique Fédérale de Lausanne
* [Climate Change and Water in Mountains: A Global Concern](https://www.coursera.org/learn/climate-changes-mountains-water) University of Geneva
* [Climate Adaptation in Africa](https://www.coursera.org/learn/climate-adaptation) University of Cape Town
* [Introduction to Faecal Sludge Management](https://www.coursera.org/learn/faecalsludge) École Polytechnique Fédérale de Lausanne
* [A Business Approach to Sustainable Landscape Restoration](https://www.coursera.org/learn/landscape-restoration-sustainable-development) Erasmus University Rotterdam
* [Жизнь в почве](https://www.coursera.org/learn/life-in-soil) National Research Tomsk State University
* [Planning for Climate Change in African Cities](https://www.coursera.org/learn/climate-change-africa) United Cities and Local Governments of Africa
* [Global Warming II: Create Your Own Models in Python](https://www.coursera.org/learn/global-warming-model) The University of Chicago
* [A Circular Economy of Metals: Towards a Sustainable Societal Metabolism](https://www.coursera.org/learn/circular-economy-metals) Universiteit Leiden
* [Geodesign: Change Your World](https://www.coursera.org/learn/geodesign) The Pennsylvania State University
* [Mobilités et véhicules électriques](https://www.coursera.org/learn/mobilites-vehicules-electriques) École des Ponts ParisTech
* [מבוא לאנרגיה מתחדשת - Introduction to Renewable Energy](https://www.coursera.org/learn/renewable-energy) Tel Aviv University
* [Global Postharvest Loss Prevention: Fundamentals, Technologies, and Actors](https://www.coursera.org/learn/postharvest) University of Illinois at Urbana-Champaign
* [Planification et Design de Systèmes et Technologies d’Assainissement](https://www.coursera.org/learn/sanitation-fr) École Polytechnique Fédérale de Lausanne
* [Systèmes d’Information Géographique - Partie 2](https://www.coursera.org/learn/sig-2) École Polytechnique Fédérale de Lausanne
* [Biosphere 2 Science for the Future of Our Planet](https://www.coursera.org/learn/biosphere-science-future) University of Arizona
* [Sustainability through Soccer: Systems-Thinking in Action](https://www.coursera.org/learn/sustainability-through-soccer) University of Virginia
* [Disaster Risk Management and Korean Policies](https://www.coursera.org/learn/disaster-risk-management-korean-policies) Yonsei University
* [Global Arctic](https://www.coursera.org/learn/global-arctic) École Polytechnique Fédérale de Lausanne
* [宇宙之旅：展现生命 (Journey of the Universe: The Unfolding of Life)](https://www.coursera.org/learn/yuzhou-zhi-lu) Yale University
* [Wasser in der Schweiz](https://www.coursera.org/learn/wasser-schweiz) University of Zurich
* [宇宙之旅：对话 (Journey of the Universe: Weaving Knowledge and Action)](https://www.coursera.org/learn/yuzhou-duihua) Yale University
* [Advanced Functional Ceramics](https://www.coursera.org/learn/advanced-functional-ceramics) Yonsei University


## physical-science-and-engineering/mechanical-engineering

* [Introduction to Engineering Mechanics](https://www.coursera.org/learn/engineering-mechanics-statics) Georgia Institute of Technology
* [Robótica](https://www.coursera.org/learn/robotica-inicial) Universidad Nacional Autónoma de México
* [Mechanics of Materials I: Fundamentals of Stress & Strain and Axial Loading](https://www.coursera.org/learn/mechanics-1) Georgia Institute of Technology
* [Materials Science: 10 Things Every Engineer Should Know](https://www.coursera.org/learn/materials-science) University of California, Davis
* [BIM Fundamentals for Engineers](https://www.coursera.org/learn/bim-fundamentals) National Taiwan University
* [3D CAD Fundamental](https://www.coursera.org/learn/3d-cad-fundamental) National Taiwan University
* [Fundamentals of Fluid Power](https://www.coursera.org/learn/fluid-power) University of Minnesota
* [BIM Application for Engineers](https://www.coursera.org/learn/bim-application) National Taiwan University
* [Applications in Engineering Mechanics](https://www.coursera.org/learn/engineering-mechanics-statics-2) Georgia Institute of Technology
* [Engineering Systems in Motion: Dynamics of Particles and Bodies in 2D Motion](https://www.coursera.org/learn/dynamics) Georgia Institute of Technology
* [Mechanics of Materials IV: Deflections, Buckling, Combined Loading & Failure Theories](https://www.coursera.org/learn/materials-structures) Georgia Institute of Technology
* [Protecting the World: Introducing Corrosion Science and Engineering](https://www.coursera.org/learn/corrosion) University of Manchester
* [Аддитивные технологии (3D-печать). Вводный курс](https://www.coursera.org/learn/additivnye-tekhnologii) Peter the Great St. Petersburg Polytechnic University
* [Introduction to Basic Vibrations](https://www.coursera.org/learn/introduction-basic-vibrations) Korea Advanced Institute of Science and Technology(KAIST)
* [Mechanics of Materials II: Thin-Walled Pressure Vessels and Torsion](https://www.coursera.org/learn/mechanics2) Georgia Institute of Technology
* [3D CAD Application](https://www.coursera.org/learn/3d-cad-application) National Taiwan University
* [Fundamentals of waves and vibrations](https://www.coursera.org/learn/fundamentals-waves-vibrations) École Polytechnique
* [Advanced Engineering Systems in Motion: Dynamics of Three Dimensional (3D) Motion](https://www.coursera.org/learn/motion-and-kinetics) Georgia Institute of Technology
* [Equilibrio, ¿por qué se caen las cosas?](https://www.coursera.org/learn/equilibrio) Pontificia Universidad Católica de Chile
* [Инновации в промышленности: мехатроника и робототехника](https://www.coursera.org/learn/innovations-in-industry-robotics) National Research Tomsk State University
* [機器人學一 (Robotics (1))](https://www.coursera.org/learn/robotics1) National Taiwan University
* [Statistical Thermodynamics: Molecules to Machines](https://www.coursera.org/learn/statistical-thermodynamics-cm) Carnegie Mellon University
* [材料力學一 (Mechanics of Materials (1))](https://www.coursera.org/learn/mechanics-of-materials-1) National Taiwan University


## physical-science-and-engineering/physics-and-astronomy

* [Astronomy: Exploring Time and Space](https://www.coursera.org/learn/astro) University of Arizona
* [Understanding Einstein: The Special Theory of Relativity](https://www.coursera.org/learn/einstein-relativity) Stanford University
* [Origens da Vida no Contexto Cósmico](https://www.coursera.org/learn/origensdavida) Universidade de São Paulo
* [Mechanics: Motion, Forces, Energy and Gravity, from Particles to Planets](https://www.coursera.org/learn/mechanics-particles-planets) UNSW Sydney (The University of New South Wales)
* [Particle Physics: an Introduction](https://www.coursera.org/learn/particle-physics) University of Geneva
* [The Science of the Solar System](https://www.coursera.org/learn/solar-system) Caltech
* [From the Big Bang to Dark Energy](https://www.coursera.org/learn/big-bang) The University of Tokyo
* [Tesoros de la Física y sus Descubridores I](https://www.coursera.org/learn/tesoros-de-la-fisica) Universidad de los Andes
* [Big History: Connecting Knowledge](https://www.coursera.org/learn/big-history) Macquarie University
* [Astrobiology and the Search for Extraterrestrial Life](https://www.coursera.org/learn/astrobiology) The University of Edinburgh
* [Archaeoastronomy](https://www.coursera.org/learn/archaeoastronomy) Politecnico di Milano
* [Imagining Other Earths](https://www.coursera.org/learn/life-on-other-planets) Princeton University
* [The Evolving Universe](https://www.coursera.org/learn/evolvinguniverse) Caltech
* [Astro 101: Black Holes](https://www.coursera.org/learn/black-holes-astro-101) University of Alberta
* [Big History - From the Big Bang until Today](https://www.coursera.org/learn/bighistory) University of Amsterdam
* [Ingeniería de Tráfico](https://www.coursera.org/learn/ingenieria-trafico) Pontificia Universidad Católica de Chile
* [Origins - Formation of the Universe, Solar System, Earth and Life](https://www.coursera.org/learn/origins-universe-solarsystem) University of Copenhagen
* [Astrobiology: Exploring Other Worlds](https://www.coursera.org/learn/astrobiology-exploring-other-worlds) University of Arizona
* [Transmission electron microscopy for materials science](https://www.coursera.org/learn/microscopy) École Polytechnique Fédérale de Lausanne
* [Statistical Mechanics: Algorithms and Computations](https://www.coursera.org/learn/statistical-mechanics) École normale supérieure
* [Estrategias para ganar. Meteorología en la vuelta al mundo](https://www.coursera.org/learn/estrategiasparaganar-meteorologia) Universitat de Barcelona
* [Mécanique quantique](https://www.coursera.org/learn/mecanique-quantique) École Polytechnique
* [AstroTech: The Science and Technology behind Astronomical Discovery](https://www.coursera.org/learn/astronomy-technology) The University of Edinburgh
* [L'Art des Structures 2 : treillis, poutres, dalles et cadres](https://www.coursera.org/learn/structures2) École Polytechnique Fédérale de Lausanne
* [Analyzing the Universe](https://www.coursera.org/learn/analyze) Rutgers the State University of New Jersey
* [Confronting The Big Questions: Highlights of Modern Astronomy](https://www.coursera.org/learn/astronomy) University of Rochester
* [Mastering Statics](https://www.coursera.org/learn/mastering-statics) The Hong Kong University of Science and Technology
* [Физика в опытах. Часть 4. Волны и оптика](https://www.coursera.org/learn/fizika-volny-optika) National Research Nuclear University MEPhI
* [История изобретений и открытий — Вторая история человечества](https://www.coursera.org/learn/istoriya-izobretenii-i-otkritii) National Research Nuclear University MEPhI
* [Thermodynamique : fondements](https://www.coursera.org/learn/thermo-base) École Polytechnique Fédérale de Lausanne
* [Элементы атомной и ядерной физики](https://www.coursera.org/learn/elementy-atomnoj-i-yadernoj-fiziki) National Research Nuclear University MEPhI
* [Strategies for winning. Meteorology in a round the world regatta](https://www.coursera.org/learn/meteorology) Universitat de Barcelona
* [L'art des structures 1 : Câbles et arcs](https://www.coursera.org/learn/structures) École Polytechnique Fédérale de Lausanne
* [普通物理學-電磁學、光學及近代物理 (General Physics (1))](https://www.coursera.org/learn/wuli) National Taiwan University
* [Cyber-Physical Systems: Modeling and Simulation](https://www.coursera.org/learn/cyber-physical-systems-1) University of California, Santa Cruz
* [Exploring Light: Hands-on Activities and Strategies for Teachers](https://www.coursera.org/learn/teach-light-color) Exploratorium
* [Mécanique : Solide Indéformable](https://www.coursera.org/learn/mecanique-solide) École Polytechnique Fédérale de Lausanne
* [Basic Notions in Physics - רעיונות מרכזיים בפיזיקה](https://www.coursera.org/learn/physics-intro) Tel Aviv University
* [Physique des particules - une introduction](https://www.coursera.org/learn/physique-particules) University of Geneva
* [Emergent Phenomena in Science and Everyday Life](https://www.coursera.org/learn/emergent-phenomena) University of California, Irvine
* [Физика как глобальный проект](https://www.coursera.org/learn/physics-global-project) National Research Nuclear University MEPhI
* [Quantum Optics 2 - Two photons and more](https://www.coursera.org/learn/quantum-optics-two-photons) École Polytechnique
* [Mécanique de Newton](https://www.coursera.org/learn/mecanique-newton) École Polytechnique Fédérale de Lausanne
* [Физика в опытах. Часть 3. Колебания и молекулярная физика](https://www.coursera.org/learn/molekulyarnaya-fizika) National Research Nuclear University MEPhI
* [基礎光學一 (Introduction to Optics (1))](https://www.coursera.org/learn/ji-chu-guang-xue) National Taiwan University
* [Изобретения, изменившие мир](https://www.coursera.org/learn/izobreteniya-izmenivshiye-mir) National Research Nuclear University MEPhI
* [Introduzione alla fisica sperimentale: elettromagnetismo, ottica, fisica moderna](https://www.coursera.org/learn/fisica-sperimentale-fisica-moderna) Politecnico di Milano
* [Thermodynamique : applications](https://www.coursera.org/learn/thermo-apps) École Polytechnique Fédérale de Lausanne
* [Vers l'infiniment petit - Voyages de l'infiniment grand à l'infiniment petit](https://www.coursera.org/learn/physique-infiniment-petit) École Polytechnique
* [走进天文学](https://www.coursera.org/learn/intro-astronomy-nju) Nanjing University
* [D'un infini à l'autre - Voyages de l'infiniment grand à l'infiniment petit](https://www.coursera.org/learn/physique-2-infinis-liens) École Polytechnique
* [Vers l'infiniment grand - Voyages de l'infiniment grand à l'infiniment petit](https://www.coursera.org/learn/physique-2-infinis-infiniment-grand) École Polytechnique
* [Mécanique du point matériel](https://www.coursera.org/learn/mecanique-point-materiel) École Polytechnique Fédérale de Lausanne
* [Introduction to Acoustics (Part 2)](https://www.coursera.org/learn/intro-to-acoustics-2) Korea Advanced Institute of Science and Technology(KAIST)
* [天文探秘](https://www.coursera.org/learn/tianwenxue) Nanjing University
* [电磁学上——恒定电场](https://www.coursera.org/learn/dianci) Peking University


## physical-science-and-engineering/research-methods

* [Understanding Research Methods](https://www.coursera.org/learn/research-methods) University of London
* [Simulation and modeling of natural processes](https://www.coursera.org/learn/modeling-simulation-natural-processes) University of Geneva
* [Драгоценные камни: диагностика и экспертиза](https://www.coursera.org/learn/kamni) Novosibirsk State University
* [Introduction to Particle Accelerators (NPAP MOOC)](https://www.coursera.org/learn/introduction-particle-accelerators) Lund University


## social-sciences/economics

* [Экономика для неэкономистов (Economics for non-economists)](https://www.coursera.org/learn/ekonomika-dlya-neekonomistov) National Research University Higher School of Economics
* [Introduction to Ancient Egypt and Its Civilization](https://www.coursera.org/learn/introancientegypt) University of Pennsylvania
* [Wonders of Ancient Egypt](https://www.coursera.org/learn/wonders-ancient-egypt) University of Pennsylvania
* [Макроэкономика (Macroeconomics)](https://www.coursera.org/learn/makrojekonomika) National Research University Higher School of Economics
* [Sustentabilidad y Economías Sociales](https://www.coursera.org/learn/sustentabilidad-economias-sociales) Universidad de Chile
* [Politics and Economics of International Energy](https://www.coursera.org/learn/global-energy) Sciences Po
* [Nuevos modelos de negocios en el siglo XXI](https://www.coursera.org/learn/modelos-negocios) Universidad Nacional Autónoma de México
* [История экономической мысли (History of Economic Thought)](https://www.coursera.org/learn/istoriya-ekonomicheskoy-mysli) National Research University Higher School of Economics
* [Основы микроэкономики (Microeconomics Principles)](https://www.coursera.org/learn/mikroekonomika) National Research University Higher School of Economics
* [Agriculture, Economics and Nature](https://www.coursera.org/learn/agriculture-economics-nature) University of Western Australia
* [Kit básico (para evitar los errores más frecuentes) de finanzas](https://www.coursera.org/learn/finanzas-basicas) Universitat Autònoma de Barcelona
* [O Poder da Macroeconomia: princípios da economia no mundo real (em Português)](https://www.coursera.org/learn/macroeconomia-pt) University of California, Irvine
* [Economics of Transition and Emerging Markets](https://www.coursera.org/learn/economics-transition-emerging-markets) National Research University Higher School of Economics
* [經濟學概論：誘因與市場（Introduction to Economics: Incentive and Markets）](https://www.coursera.org/learn/economics) National Taiwan University
* [The Korean Economic Development](https://www.coursera.org/learn/korean-economy) Yonsei University
* [實驗經濟學 (Experimental Economics: Behavioral Game Theory)](https://www.coursera.org/learn/shiyan-jingji-xue) National Taiwan University
* [China’s Economic Transformation Part 1: Economic Reform and Growth in China](https://www.coursera.org/learn/econtransform1) The Hong Kong University of Science and Technology
* [Understanding Russian Economy. Problems of Transition](https://www.coursera.org/learn/economy-russia-transition) National Research University Higher School of Economics
* [Economic Growth and Distributive Justice Part II - Maximize Social Wellbeing](https://www.coursera.org/learn/economic-growth-part-2) Tel Aviv University


## social-sciences/education

* [What Is Contemporary Art?](https://www.coursera.org/learn/contemporary-art) The Museum of Modern Art
* [Cómo hacer una tesis](https://www.coursera.org/learn/como-hacer-una-tesis) Universidad Nacional Autónoma de México
* [The Science of Success: What Researchers Know that You Should Know](https://www.coursera.org/learn/success) University of Michigan
* [Magic in the Middle Ages](https://www.coursera.org/learn/magic-middle-ages) Universitat de Barcelona
* [Hacia una práctica constructivista en el aula](https://www.coursera.org/learn/aulaconstructivista) Pontificia Universidad Católica de Chile
* [Supporting children with difficulties in reading and writing](https://www.coursera.org/learn/dyslexia-difficulties) University of London
* [Transmedia Storytelling: Narrative worlds, emerging technologies, and global audiences](https://www.coursera.org/learn/transmedia-storytelling) UNSW Sydney (The University of New South Wales)
* [Développement psychologique de l'enfant](https://www.coursera.org/learn/enfant-developpement) University of Geneva
* [Teaching Character and Creating Positive Classrooms](https://www.coursera.org/learn/teaching-character) Relay Graduate School of Education
* [Usos Didácticos del Cine: Introducción al Análisis](https://www.coursera.org/learn/usos-didacticos-del-cine) Universidad Nacional Autónoma de México
* [Representaciones culturales de las sexualidades](https://www.coursera.org/learn/representaciones-culturales) Universitat Autònoma de Barcelona
* [Understanding child development: from synapse to society](https://www.coursera.org/learn/child-development) Utrecht University
* [Teaching EFL/ESL Reading: A Task Based Approach](https://www.coursera.org/learn/esl-reading) University of London
* [Art & Inquiry: Museum Teaching Strategies For Your Classroom](https://www.coursera.org/learn/artinquiry) The Museum of Modern Art
* [Get Interactive: Practical Teaching with Technology](https://www.coursera.org/learn/getinmooc) University of London
* [What future for education?](https://www.coursera.org/learn/future-education) University of London
* [Claves para la innovación en la docencia universitaria](https://www.coursera.org/learn/innovacion-docencia-universitaria) Universitat de Barcelona
* [Docencia para la capacitación laboral y el aprendizaje a lo largo de la vida.](https://www.coursera.org/learn/docencia-capacitacion-laboral) Universidad de Chile
* [Atrévete a innovar tu enseñanza con pensamiento de diseño](https://www.coursera.org/learn/innovacioneducativa) Universidad Nacional Autónoma de México
* [Disability Inclusion in Education: Building Systems of Support](https://www.coursera.org/learn/disability-inclusion-education) University of Cape Town
* [Get Organized: How to be a Together Teacher](https://www.coursera.org/learn/together-teacher) Relay Graduate School of Education
* [Challenging Forensic Science: How Science Should Speak to Court](https://www.coursera.org/learn/challenging-forensic-science) University of Lausanne
* [Learning, Knowledge, and Human Development](https://www.coursera.org/learn/learning-knowledge-human-development) University of Illinois at Urbana-Champaign
* [Children Acquiring Literacy Naturally](https://www.coursera.org/learn/children-literacy) University of California, Santa Cruz
* [Research Data Management and Sharing](https://www.coursera.org/learn/data-management) The University of North Carolina at Chapel Hill
* [Writing your World: Finding yourself in the academic space](https://www.coursera.org/learn/writing-your-world) University of Cape Town
* [Orchestrating Whole Classroom Discussion](https://www.coursera.org/learn/classdiscussion) University of Pennsylvania
* [Copyright for Educators & Librarians](https://www.coursera.org/learn/copyright-for-education) Duke University
* [American Deaf Culture](https://www.coursera.org/learn/deaf-culture) University of Houston System
* [Serious Gaming](https://www.coursera.org/learn/serious-gaming) Erasmus University Rotterdam
* [Aboriginal Worldviews and Education](https://www.coursera.org/learn/aboriginal-education) University of Toronto
* [The Dynamic Earth: A Course for Educators](https://www.coursera.org/learn/earth-amnh) American Museum of Natural History
* [Studying Cities: Social Science Methods for Urban Research](https://www.coursera.org/learn/studying-cities-social-science-methods-for-urban-research) Erasmus University Rotterdam
* [Blended Learning: Personalizing Education for Students](https://www.coursera.org/learn/blending-learning-personalization) New Teacher Center
* [Assessment in Higher Education: Professional Development for Teachers](https://www.coursera.org/learn/assessment-higher-education) Erasmus University Rotterdam
* [Evolution: A Course for Educators](https://www.coursera.org/learn/teaching-evolution) American Museum of Natural History
* [Jugar y Aprender Matemática en aulas heterogéneas](https://www.coursera.org/learn/matematica-aulas-heterogeneas) Universidad Austral
* [Critical Issues in Urban Education](https://www.coursera.org/learn/urban-education) The University of Chicago
* [Assessment for Learning](https://www.coursera.org/learn/assessmentforlearning) University of Illinois at Urbana-Champaign
* [علم النجاح: ما يجب أن تعرفه من الباحثين](https://www.coursera.org/learn/success-ar) University of Michigan
* [Foundations of Teaching for Learning: Developing Relationships](https://www.coursera.org/learn/teacher-relationships) Commonwealth Education Trust
* [K-12 Blended & Online Learning](https://www.coursera.org/learn/k-12-online-education) University System of Georgia
* [Antisemitism: From Its Origins to the Present](https://www.coursera.org/learn/antisemitism) Yad Vashem
* [Doping : Sports, Organizations and Sciences](https://www.coursera.org/learn/doping) University of Lausanne
* [Literacy Teaching and Learning: Aims, Approaches and Pedagogies](https://www.coursera.org/learn/literacy-teaching-learning) University of Illinois at Urbana-Champaign
* [Severe to Profound Intellectual Disability: Circles of Care and Education](https://www.coursera.org/learn/intellectual-disability-care-education) University of Cape Town
* [Social Pedagogy across Europe](https://www.coursera.org/learn/social-pedagogy-europe) Universitat Autònoma de Barcelona
* [La enseñanza de las Ciencias Naturales en la escuela primaria](https://www.coursera.org/learn/ensenar-ciencias-naturales) Universidad Austral
* [Disability Awareness and Support](https://www.coursera.org/learn/disability-awareness) University of Pittsburgh
* [Teaching Popular Music in the Classroom](https://www.coursera.org/learn/teaching-popular-music) Berklee College of Music
* [Ubiquitous Learning and Instructional Technologies](https://www.coursera.org/learn/ubiquitouslearning) University of Illinois at Urbana-Champaign
* [El trabajo por proyectos en escuelas de contextos rurales](https://www.coursera.org/learn/trabajo-proyectos-escuelas-rurales) Universidad Austral
* [La alfabetización temprana en contextos rurales](https://www.coursera.org/learn/alfabetizacion-temprana-contextos-rurales) Universidad Austral
* [Multimodal Literacies: Communication and Learning in the Era of Digital Media](https://www.coursera.org/learn/multimodal-literacies) University of Illinois at Urbana-Champaign
* [Frontières en tous genres](https://www.coursera.org/learn/geographie-politique-culturelle-frontieres) University of Geneva
* [The Place of Music in 21st Century Education](https://www.coursera.org/learn/music-education) The University of Sydney
* [社会调查与研究方法 （上）Methodologies in Social Research (Part I)](https://www.coursera.org/learn/shehu-yanjiu-fangfa) Peking University
* [La science forensique au tribunal: témoin digne de foi ?](https://www.coursera.org/learn/science-forensique-tribunal) University of Lausanne
* [Accessibility to the Scenic Arts](https://www.coursera.org/learn/accessibility-scenic-arts) Universitat Autònoma de Barcelona
* [Negotiating Learner Differences: Towards Productive Diversity in Learning](https://www.coursera.org/learn/learnerdifferences) University of Illinois at Urbana-Champaign
* [Gestão para a Aprendizagem: Módulo Gestão Estratégica](https://www.coursera.org/learn/gestao-escolar) Fundação Lemann
* [Faster Together, Enhancing the Recruitment of Minorities in Clinical Trials](https://www.coursera.org/learn/recruitment-minorities-clinical-trials) Vanderbilt University
* [My Favorite Lectures @ HKUST](https://www.coursera.org/learn/my-favorite-lectures-hkust) The Hong Kong University of Science and Technology
* [Service Transformed: Lessons in U.S. Veteran Centered Care](https://www.coursera.org/learn/va-health-care) University of Michigan
* [Учительський коучинг: сприяння розвитку сталих змін](https://www.coursera.org/learn/uchytelskyy-kouchynh) Match Teacher Residency
* [Explorando os recursos educacionais da Khan Academy](https://www.coursera.org/learn/khanacademy) Fundação Lemann
* [Aprenda a ensinar programação com o Programaê!](https://www.coursera.org/learn/programae) Fundação Lemann
* [L’antisémitisme : De ses origines à nos jours](https://www.coursera.org/learn/antisemitisme) Yad Vashem
* [Social Science Approaches to the Study of Chinese Society Part 2](https://www.coursera.org/learn/social-science-research-chinese-society) The Hong Kong University of Science and Technology
* [社会调查与研究方法 （下）Methodologies in Social Research (Part 2)](https://www.coursera.org/learn/shehui-diaocha-yanjiu-fangfa) Peking University
* [网络课程与学习评价](https://www.coursera.org/learn/wangluo-kecheng-xuexi-pingjia) Nanjing University


## social-sciences/governance-and-society

* [Global Diplomacy – Diplomacy in the Modern World](https://www.coursera.org/learn/global-diplomacy) University of London
* [Epidemics, Pandemics and Outbreaks](https://www.coursera.org/learn/epidemic-pandemic-outbreak) University of Pittsburgh
* [Introduction to Neuroeconomics: How the Brain Makes Decisions](https://www.coursera.org/learn/neuroeconomics) National Research University Higher School of Economics
* [Democracia y decisiones públicas. Introducción al análisis de políticas públicas](https://www.coursera.org/learn/democracia) Universitat Autònoma de Barcelona
* [Terrorism and Counterterrorism: Comparing Theory and Practice](https://www.coursera.org/learn/terrorism) Universiteit Leiden
* [Classical Sociological Theory](https://www.coursera.org/learn/classical-sociological-theory) University of Amsterdam
* [Anticorrupción: Introducción a conceptos y perspectiva práctica](https://www.coursera.org/learn/anticorrupcion-introduccion) Universidad Nacional Autónoma de México
* [Competencias Laborales: Perfiles, Evaluación y Capacitación.](https://www.coursera.org/learn/competencias-lab) Universidad de Chile
* [Geopolítica y gobernanza global: riesgos y oportunidades](https://www.coursera.org/learn/geopoliticaygobernanzaglobal) ESADE Business and Law School
* [The Sustainable Development Goals – A global, transdisciplinary vision for the future](https://www.coursera.org/learn/global-sustainable-development) University of Copenhagen
* [Periodismo digital y combate a las fake news](https://www.coursera.org/learn/periodismo-digital) Universidad Nacional Autónoma de México
* [Global Diplomacy: the United Nations in the World](https://www.coursera.org/learn/global-diplomacy-un) University of London
* [Paradoxes of War](https://www.coursera.org/learn/war) Princeton University
* [Introduction to Communication Science](https://www.coursera.org/learn/communication) University of Amsterdam
* [Introduction to Contemporary Geopolitics](https://www.coursera.org/learn/contemprorary-geopolitics) National Research University Higher School of Economics
* [Arts and Culture Strategy](https://www.coursera.org/learn/arts-culture-strategy) University of Pennsylvania
* [¿Cómo llegamos aquí? Una historia del poder en México](https://www.coursera.org/learn/historia-de-mexico) Universidad Nacional Autónoma de México
* [América Latina en los cambios internacionales: amenazas y oportunidades.](https://www.coursera.org/learn/america-latina) Universidad de Chile
* [Acuerdos globales para el desarrollo sostenible](https://www.coursera.org/learn/acuerdos-globales) Universidad Nacional Autónoma de México
* [Los gobiernos locales como actores internacionales](https://www.coursera.org/learn/gobiernos-locales) Universidad Nacional Autónoma de México
* [The Changing Global Order](https://www.coursera.org/learn/changing-global-order) Universiteit Leiden
* [Sports and Society](https://www.coursera.org/learn/sports-society) Duke University
* [Roman Art and Archaeology](https://www.coursera.org/learn/roman-art-archaeology) University of Arizona
* [Global Energy and Climate Policy](https://www.coursera.org/learn/globalenergyandclimatepolicy) University of London
* [Sustainable Tourism – promoting environmental public health](https://www.coursera.org/learn/sustainable-tourism) University of Copenhagen
* [Discover Best Practice Farming for a Sustainable 2050](https://www.coursera.org/learn/best-practice-farming-sustainable-2050) University of Western Australia
* [Geopolitics of Europe](https://www.coursera.org/learn/geopolitics-europe) Sciences Po
* [Политическая география](https://www.coursera.org/learn/politicheskaya-geografiya) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [The Social Context of Mental Health and Illness](https://www.coursera.org/learn/mental-health) University of Toronto
* [The Cosmopolitan Medieval Arabic World](https://www.coursera.org/learn/medieval-arabia) Universiteit Leiden
* [Cities are back in town : urban sociology for a globalizing urban world](https://www.coursera.org/learn/urban-development) Sciences Po
* [Chinese Politics Part 1 – China and Political Science](https://www.coursera.org/learn/chinesepolitics1) The Hong Kong University of Science and Technology
* [La verde y sus verdades](https://www.coursera.org/learn/verde-verdades) Universidad Nacional Autónoma de México
* [Security & Safety Challenges in a Globalized World](https://www.coursera.org/learn/security-safety-globalized-world) Universiteit Leiden
* [Ciudades en crisis y nuevas políticas urbanas](https://www.coursera.org/learn/ciudades-politicas-urbanas) Universitat Autònoma de Barcelona
* [Political Economy of Institutions and Development](https://www.coursera.org/learn/political-economy) Universiteit Leiden
* [Water Resources Management and Policy](https://www.coursera.org/learn/water-management) University of Geneva
* [America's Written Constitution](https://www.coursera.org/learn/written-constitution) Yale University
* [Network Dynamics of Social Behavior](https://www.coursera.org/learn/networkdynamics) University of Pennsylvania
* [America Through Foreign Eyes](https://www.coursera.org/learn/america-through-foreign-eyes) Rice University
* [Géopolitique de l'Europe](https://www.coursera.org/learn/geopolitique) Sciences Po
* [Refugees in the 21st Century](https://www.coursera.org/learn/refugees-21st-century) University of London
* [The Economics of Agro-Food Value Chains](https://www.coursera.org/learn/valuechains) Technische Universität München (TUM)
* [Экономическая социология](https://www.coursera.org/learn/ekonomicheskaya-sociologiya) National Research University Higher School of Economics
* [Gender, Family, and Social Change in Contemporary South Korea](https://www.coursera.org/learn/social-change-korea) Yonsei University
* [Genre : quels enjeux ? Violences, globalisation, biomédecine, sexualités.](https://www.coursera.org/learn/genre) University of Geneva
* [Институциональная экономика (Institutional economics)](https://www.coursera.org/learn/institutional-economics) National Research University Higher School of Economics
* [Сравнительная политика (Comparative Politics)](https://www.coursera.org/learn/politika-sravnitelnaja) National Research University Higher School of Economics
* [Water Supply and Sanitation Policy in Developing Countries Part 1: Understanding Complex Problems](https://www.coursera.org/learn/water) University of Manchester
* [Introdução à Economia do Trabalho: Teorias e Políticas](https://www.coursera.org/learn/economia-do-trabalho) Universidade Estadual de Campinas
* [Soul Beliefs: Causes and Consequences - Unit 1: Historical Foundations](https://www.coursera.org/learn/soulbeliefs) Rutgers the State University of New Jersey
* [Risk in Modern Society](https://www.coursera.org/learn/risk-in-modern-society) Universiteit Leiden
* [Afrique et mondialisation, regards croisés](https://www.coursera.org/learn/afrique-mondialisation) Sciences Po
* [Cultural Competence - Aboriginal Sydney](https://www.coursera.org/learn/cultural-competence-aboriginal-sydney) The University of Sydney
* [The City and You: Find Your Best Place](https://www.coursera.org/learn/city-and-you-find-best-place) University of Toronto
* [Introducción al estudio de los bienes comunes](https://www.coursera.org/learn/estudio-bienes-comunes) Universidad Nacional Autónoma de México
* [Understanding 9/11: Why 9/11 Happened & How Terrorism Affects Our World Today](https://www.coursera.org/learn/911-attack) Duke University
* [Age of Jefferson](https://www.coursera.org/learn/ageofjefferson) University of Virginia
* [Humanitarian communication : Addressing key challenges](https://www.coursera.org/learn/humanitarian-communication) University of Geneva
* [Mobilité et urbanisme](https://www.coursera.org/learn/mobiurba) École Polytechnique Fédérale de Lausanne
* [Israel State and Society](https://www.coursera.org/learn/israel) Hebrew University of Jerusalem
* [Research for Impact](https://www.coursera.org/learn/research-for-impact) University of Cape Town
* [¿Cómo (nos) cambia la Tecnología?](https://www.coursera.org/learn/comonoscambialatecnologia) Universidad de Chile
* [The Kennedy Half Century](https://www.coursera.org/learn/kennedy) University of Virginia
* [Giving 2.0: The MOOC](https://www.coursera.org/learn/philanthropist) Stanford University
* [Cartographie thématique](https://www.coursera.org/learn/cartographie) École normale supérieure
* [From Climate Science to Action](https://www.coursera.org/learn/climate-science) The World Bank Group
* [Cities are back in town : sociología urbana para un mundo globalizado](https://www.coursera.org/learn/desarrollo-urbano) Sciences Po
* [A la recherche du Grand Paris](https://www.coursera.org/learn/grand-paris-metropole) Sciences Po
* [Villes africaines: Environnement et enjeux de développement durable](https://www.coursera.org/learn/environnement-urbain-afrique) École Polytechnique Fédérale de Lausanne
* [African cities : An Introduction to Urban Planning](https://www.coursera.org/learn/african-cities1) École Polytechnique Fédérale de Lausanne
* [Heritage under Threat](https://www.coursera.org/learn/heritage-protection) Universiteit Leiden
* [Religions and Society in China](https://www.coursera.org/learn/religions-society-china) National Research University Higher School of Economics
* [From Freedom Rides to Ferguson: Narratives of Nonviolence in the American Civil Rights Movement](https://www.coursera.org/learn/nonviolence) Emory University
* [Les Partenariats Public-Privé (PPP): Comment offrir de meilleures infrastructures pour les services publics](https://www.coursera.org/learn/partenariats-public-prive) The World Bank Group
* [Cities are back in town : sociologie urbaine pour un monde globalisé](https://www.coursera.org/learn/developpement-urbain) Sciences Po
* [Measuring Causal Effects in the Social Sciences](https://www.coursera.org/learn/causal-effects) University of Copenhagen
* [Bajemos la temperatura: De la ciencia climática a la acción](https://www.coursera.org/learn/cambios-temperatura) The World Bank Group
* [Chinese Politics Part 2 – China and the World](https://www.coursera.org/learn/chinese-politics-2) The Hong Kong University of Science and Technology
* [Financing Infrastructure in African Cities](https://www.coursera.org/learn/financing-infrastructure-in-african-cities) United Cities and Local Governments of Africa
* [Planification des mobilités](https://www.coursera.org/learn/planification-mobilites) École Polytechnique Fédérale de Lausanne
* [Les partenariats qui changent le monde : alliances innovantes entre entreprises et associations](https://www.coursera.org/learn/partenariats-qui-changent-le-monde) ESSEC Business School
* [Villes africaines I: Introduction à la planification urbaine](https://www.coursera.org/learn/villes-africaines-1) École Polytechnique Fédérale de Lausanne
* [Federalism & Decentralization: Evaluating Africa's Track Record](https://www.coursera.org/learn/decentralization-africa) Universiteit Leiden
* [Patrick Henry: Forgotten Founder](https://www.coursera.org/learn/henry) University of Virginia
* [The Rooseveltian Century](https://www.coursera.org/learn/roosevelt) Universiteit Leiden
* [فهم صنع السياسات الاقتصادية](https://www.coursera.org/learn/economic-policy-ar) IE Business School
* [Searching for the Grand Paris](https://www.coursera.org/learn/grand-paris-metropolis) Sciences Po
* [L’Egitto prima e dopo i faraoni. Dalla nascita dello Stato (3000 a.C. ca.) alle prime comunità cristiane (IV secolo d.C.)](https://www.coursera.org/learn/egitto) Sapienza University of Rome
* [Understanding the Australian economy: An introduction to macroeconomic and financial policies](https://www.coursera.org/learn/australian-economy) The University of Sydney
* [Villes africaines: Mobilités et transports urbains](https://www.coursera.org/learn/mobilite-afrique) École Polytechnique Fédérale de Lausanne
* [Water Supply and Sanitation Policy in Developing Countries Part 2: Developing Effective Interventions](https://www.coursera.org/learn/water-part-2) University of Manchester
* [少年福利與權利 (Welfare and Rights of Youth)](https://www.coursera.org/learn/shaonian-fuli) National Taiwan University
* [人群与网络](https://www.coursera.org/learn/renqun-wangluo) Peking University
* [Violence Against Healthcare](https://www.coursera.org/learn/violence-against-healthcare) University of Geneva
* [Villes africaines : Restructuration des quartiers précaires](https://www.coursera.org/learn/bidonvilles) École Polytechnique Fédérale de Lausanne
* [Les alliances qui changent les territoires : partenariats entre acteurs publics, acteurs privés et structures d'intérêt général pour le bien commun](https://www.coursera.org/learn/les-alliances-qui-changent-les-territoires) ESSEC Business School
* ["Espace mondial" الرؤية الفرنسية للدراسات العالمية](https://www.coursera.org/learn/espace-mondial-ar) Sciences Po
* [In the footsteps of Zika… approaching the unknown](https://www.coursera.org/learn/zika) University of Geneva
* [Bridging healthcare and society](https://www.coursera.org/learn/healthcare-and-society) National Research Tomsk State University
* [Introduction to the Orbital Perspective](https://www.coursera.org/learn/orbitalperspective) University of Arizona
* ["Making" Progress Teach-Out](https://www.coursera.org/learn/makingprogress) Emory University
* [Why Iowa? A Primer on Primaries and Caucuses Teach-Out](https://www.coursera.org/learn/why-iowa-a-primer-on-primaries-and-caucuses) University of Michigan
* [家庭社会学导论](https://www.coursera.org/learn/jiating-shehui-xue) Peking University


## social-sciences/law

* [An Introduction to American Law](https://www.coursera.org/learn/american-law) University of Pennsylvania
* [A Law Student's Toolkit](https://www.coursera.org/learn/law-student) Yale University
* [Introduction to International Criminal Law](https://www.coursera.org/learn/international-criminal-law) Case Western Reserve University
* [Introduction to English Common Law](https://www.coursera.org/learn/intro-common-law) University of London
* [American Contract Law I](https://www.coursera.org/learn/contracts-1) Yale University
* [Rethinking International Tax Law](https://www.coursera.org/learn/international-taxation) Universiteit Leiden
* [International Humanitarian Law in Theory and Practice](https://www.coursera.org/learn/international-humanitarian-law) Universiteit Leiden
* [International Law in Action: the Arbitration of International Disputes](https://www.coursera.org/learn/arbitration-international-disputes) Universiteit Leiden
* [Introduction aux Droits de l’Homme](https://www.coursera.org/learn/droits-de-lhomme) University of Geneva
* [Internet Giants: The Law and Economics of Media Platforms](https://www.coursera.org/learn/internetgiants) The University of Chicago
* [International Law in Action: A Guide to the International Courts and Tribunals in The Hague](https://www.coursera.org/learn/international-law-in-action) Universiteit Leiden
* [European Business Law: Understanding the Fundamentals](https://www.coursera.org/learn/european-law-fundamentals) Lund University
* [International Law In Action: Investigating and Prosecuting International Crimes](https://www.coursera.org/learn/international-law-in-action-2) Universiteit Leiden
* [Ценные бумаги: правовое регулирование](https://www.coursera.org/learn/cennye-bumagi-pravovoe-regulirovanie) National Research University Higher School of Economics
* [Introduction to Key Constitutional Concepts and Supreme Court Cases](https://www.coursera.org/learn/constitution) University of Pennsylvania
* [Rédaction de contrats](https://www.coursera.org/learn/contrats) University of Geneva
* [Constitutional Struggles in the Muslim World](https://www.coursera.org/learn/muslim-world) University of Copenhagen
* [Human Rights for Open Societies](https://www.coursera.org/learn/humanrights) Utrecht University
* [EU policy and implementation: making Europe work!](https://www.coursera.org/learn/eu-making-europe-work) Universiteit Leiden
* [After the Arab Spring – Democratic Aspirations and State Failure](https://www.coursera.org/learn/after-the-arab-spring) University of Copenhagen
* [European Business Law: Doing Business in Europe](https://www.coursera.org/learn/eu-law-doing-business) Lund University
* [Contratación y mercado digital. Aspectos legales y otras cuestiones de interés](https://www.coursera.org/learn/mercado-digital) Universitat Autònoma de Barcelona
* [America's Unwritten Constitution](https://www.coursera.org/learn/unwritten-constitution) Yale University
* [Corporate governance. Mitos y realidades](https://www.coursera.org/learn/corporate-governance-mitos-realidades) Universitat Autònoma de Barcelona
* [International Water Law](https://www.coursera.org/learn/international-water-law) University of Geneva
* [Making Successful Decisions through the Strategy, Law & Ethics Model](https://www.coursera.org/learn/strategy-law-ethics) University of Michigan
* [American Contract Law II](https://www.coursera.org/learn/contracts-2) Yale University
* [Property and Liability: An Introduction to Law and Economics](https://www.coursera.org/learn/property-law-and-economics) Wesleyan University
* [Economic Growth and Distributive Justice Part I -The Role of the State](https://www.coursera.org/learn/economic-growth-part-1) Tel Aviv University
* [European Business Law: Competing in Europe](https://www.coursera.org/learn/eu-competition-law) Lund University
* [Citizenship and the Rule of Law](https://www.coursera.org/learn/citizenship-rule-of-law) University of London
* [Historia de las reglas del fútbol en Inglaterra y en Argentina](https://www.coursera.org/learn/historia-reglas-futbol) Universidad Austral
* [Международные финансы](https://www.coursera.org/learn/mezhdunarodnyye-finansy) Moscow State Institute of International Relations (MGIMO) / МГИМО (Московский государственный институт международных отношений МИД России)
* [论文写作初阶（Academic Writing and Research）](https://www.coursera.org/learn/lunwen-xiezuo-chujie) Peking University
* [Gestion et Politique de l'eau](https://www.coursera.org/learn/gestion-eau) University of Geneva
* [Magna Carta and its Legacies: Freedom and protest](https://www.coursera.org/learn/magna-carta) University of London
* [Cross-border road transport in EU law context](https://www.coursera.org/learn/transport-eu-law) Erasmus University Rotterdam
* [刑法学总论 Criminal Law](https://www.coursera.org/learn/xingfa-xue-zong-lun) Peking University
* [Droit International de l'Eau Douce](https://www.coursera.org/learn/droit-international-eau-douce) University of Geneva


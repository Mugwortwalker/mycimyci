Mycodo
======

Environmental Regulation System

Latest version: 8.12.9

Mycodo is open source software for the Raspberry Pi that couples inputs and outputs in interesting ways to sense and manipulate the environment.

|Build Status| |Codacy Badge| |Translation Badge| |DOI|

Support
-------

Documentation
~~~~~~~~~~~~~

`Mycodo Manual <https://kizniche.github.io/Mycodo>`__ (`PDF <https://github.com/kizniche/Mycodo/raw/master/docs/mycodo-manual.pdf>`__)

`Mycodo API <https://kizniche.github.io/Mycodo/mycodo-api.html>`__ (Version: v1)

`Mycodo Wiki <https://github.com/kizniche/Mycodo/wiki>`__

`Mycodo Custom Module Repository <https://github.com/kizniche/Mycodo-custom>`__

`Mycodo Support Android App <https://play.google.com/store/apps/details?id=com.mycodo.mycododocs>`__

Discussion
~~~~~~~~~~

`Mycodo Issues (Bug Reports/Feature Requests) <https://github.com/kizniche/Mycodo/issues>`__

`Mycodo Forum <https://forum.kylegabriel.com>`__ (the `old forum <https://kylegabriel.com/forum>`__ is being phased out, registration closed)

`Mycodo Discord <https://discord.gg/kmDNky4ZHZ>`__

Bug in the Mycodo Software
~~~~~~~~~~~~~~~~~~~~~~~~~~

If you believe there is a bug in the Mycodo software, first search through the github `Issues <https://github.com/kizniche/Mycodo/issues>`__ and see if your issue has already recently been discussed or resolved. If your issue is novel or significantly more recent than a similar one, you should create a `New Issue <https://github.com/kizniche/Mycodo/issues/new>`__. When creating a new issue, make sure to read all information in the issue template and follow the instructions. Replace the template text with the information being requested (e.g. "step 1" under "Steps to Reproduce the issue" should be replaced with the actual steps to reproduce the issue). The more information you provide, the easier it is to reproduce and diagnose the issue. If the issue is not able to reproduced because not enough information is provided, it may delay or prevent solving the issue.

Donate
------

I have always made Mycodo free and I don't intend on changing that. However, if you find Mycodo useful and would like to support its continued development, please consider becoming a sponsor at `github.com/sponsors/kizniche <https://github.com/sponsors/kizniche>`__ or donate at `kylegabriel.com/donate <https://kylegabriel.com/donate>`__.

--------------

.. contents:: Table of Contents
   :depth: 1

Features
--------

-  `Inputs <https://kizniche.github.io/Mycodo/Inputs/>`__ that record measurements from sensors, GPIO pin states, analog-to-digital converters, and more (or create your own `Custom Inputs <#custom-inputs>`__). See all `Supported Inputs <https://kizniche.github.io/Mycodo/Supported-Inputs-By-Measurement/>`__.
-  `Outputs <https://kizniche.github.io/Mycodo/Outputs/>`__ that perform actions such as switching GPIO pins high/low, generating PWM signals, executing shell scripts and Python code, and more (or create your own `Custom Outputs <#custom-outputs>`__). See all `Supported Outputs <https://kizniche.github.io/Mycodo/Supported-Outputs/>`__.
-  `Functions <https://kizniche.github.io/Mycodo/Functions/>`__ that perform tasks, such as coupling Inputs and Outputs in interesting ways, such as `PID controllers <https://kizniche.github.io/Mycodo/Functions/#pid-controller>`__, `Conditional Controllers <https://kizniche.github.io/Mycodo/Functions/#conditional>`__, `Trigger Controllers <https://kizniche.github.io/Mycodo/Functions/#trigger>`__, to name a few (or create your own `Custom Functions <https://kizniche.github.io/Mycodo/Functions/#custom-functions>`__). See all `Supported Functions <https://kizniche.github.io/Mycodo/Supported-Functions/>`__.
-  `Web Interface <https://kizniche.github.io/Mycodo/About/#web-interface>`__ for securely accessing Mycodo using a web browser on your local network or anywhere in the world with an internet connection, to view and configure the system, which includes several light and dark themes.
-  `Dashboards <https://kizniche.github.io/Mycodo/Data-Viewing/#dashboard>`__ that display configurable widgets, including interactive live and historical graphs, gauges, output state indicators, measurements, and more (or create your own `Custom Widgets <https://kizniche.github.io/Mycodo/Widgets/#custom-widgets>`__). See all `Supported Widgets <https://kizniche.github.io/Mycodo/Supported-Widgets/>`__.
-  `Alert Notifications <https://kizniche.github.io/Mycodo/Alerts/>`__ to send emails when measurements reach or exceed user-specified thresholds, important for knowing immediately when issues arise.
-  `Setpoint Tracking <https://kizniche.github.io/Mycodo/Methods/>`__ for changing a PID controller setpoint over time, for use with things like terrariums, reflow ovens, thermal cyclers, sous-vide cooking, and more.
-  `Notes <https://kizniche.github.io/Mycodo/Notes/>`__ to record events, alerts, and other important points in time, which can be overlaid on graphs to visualize events with your measurement data.
-  `Cameras <https://kizniche.github.io/Mycodo/Camera/>`__ for remote live streaming, image capture, and time-lapse photography.
-  `Energy Usage Measurement <https://kizniche.github.io/Mycodo/Energy-Usage/>`__ for calculating and tracking power consumption and cost over time.
-  `Upgrade System <https://kizniche.github.io/Mycodo/Upgrade-Backup-Restore/>`__ to easily upgrade the Mycodo system to the latest release to get the newest features or restore to a previously-backed up version.
-  `Translations <https://kizniche.github.io/Mycodo/Translations/>`__ that enable the web interface to be presented in different `Languages <https://github.com/kizniche/Mycodo#features>`__.

.. image:: https://kylegabriel.com/projects/wp-content/uploads/sites/3/2020/06/Screenshot_2020-04-25-hydra-Default-Dashboard-Mycodo-8-4-0-dashboard_2.png
   :target: https://kylegabriel.com/projects/wp-content/uploads/sites/3/2020/06/Screenshot_2020-04-25-hydra-Default-Dashboard-Mycodo-8-4-0-dashboard_2.png

Figure: `Automated Hydroponic System Build <https://kylegabriel.com/projects/2020/06/automated-hydroponic-system-build.html>`__

--------------

Uses
----

Originally developed to cultivate edible mushrooms, Mycodo has evolved to do much more. Here are a few things that have been done with Mycodo:

My projects
~~~~~~~~~~~

-  `Mushroom Cultivation Automation <https://kylegabriel.com/projects/2021/09/mushroom-cultivation-automation.html>`__ (`Archive <https://archive.is/HUtdp>`__)
-  `Hydroponic System Automation <https://kylegabriel.com/projects/2020/06/automated-hydroponic-system-build.html>`__ (`Archive <http://archive.is/mB2zc>`__)
-  `Mushroom cultivation <https://kylegabriel.com/projects/2015/04/mushroom-cultivation-revisited.html>`__ (`Archive <http://archive.is/J92Xa>`__)
-  `Ground-based plant cultivation <https://www.youtube.com/watch?v=QNCx_VE7D-8>`__
-  `Maintaining honey bee apiary homeostasis <https://kylegabriel.com/projects/2015/12/environmentally-controlled-apiary.html>`__ (`Archive <http://archive.is/RLo6n>`__)
-  `Maintaining humidity in an underground artificial bat cave <https://kylegabriel.com/projects/2015/10/artificial-bat-cave.html>`__ (`Archive <http://archive.is/QIJ5G>`__)
-  `Remote radiation monitoring and mapping <https://kylegabriel.com/projects/2019/08/remote-radiation-monitoring.html>`__ (`Archive <http://archive.is/PF44Z>`__)
-  `Cooking sous-vide <https://hackaday.io/project/11997-mycodo-environmental-regulation-system/log/45733-sous-vide-pid-tuning-and-the-unexpected-electrical-fire>`__ (`Archive <http://archive.is/Mx52U>`__)
-  `Maintaining a light schedule and regulating humidity <https://fieldstation.kennesaw.edu/summer-days-2020.php#2020_07_16_gabriel_chestnut>`__, ramping from 90 % to 50 % over a 4 week period to acclimatize micropropagated American chestnut plantlets from laboratory to ambient outdoor conditions (`Archive <http://archive.is/Jp60P>`__)

Featured
~~~~~~~~

.. image:: https://kylegabriel.com/projects/wp-content/uploads/sites/3/2021/09/MushroomCultivation_512x288.jpg
   :target: https://www.youtube.com/watch?v=z41Wy5ZF4O8

.. image:: https://kylegabriel.com/projects/wp-content/uploads/sites/3/2020/07/VID_PROJ_HYDRO_512x288.jpg
   :target: https://www.youtube.com/watch?v=nyqykZK2Ev4

Projects of others
~~~~~~~~~~~~~~~~~~

-  Maintaining aquatic systems (e.g. fish, hydroponic, aquaponic)
-  Maintaining terrarium, herpetarium, and vivarium environments
-  Incubating young animals and eggs
-  Aging cheese
-  Dry-aging, curing, and smoking meat (`Link 1 <http://www.charcuterie-worst.nl/forum/index.php/topic,425.0.html>`__ (`Archive <http://archive.is/NHKqp>`__), `Link 2 <https://www.floriske.nl/wordpress/2019/06/meat-curing-cabinet/>`__ (`Archive <https://archive.ph/57ouJ>`__))
-  Fermenting beer, food, and tobacco
-  Controlling reflow ovens
-  Culturing microorganisms
-  `Treating agricultural waste water <https://projects.sare.org/project-reports/gne17-158/>`__ (`Archive <http://archive.is/enJQs>`__, `Publication <https://pubs.acs.org/doi/pdf/10.1021/acsestwater.0c00234>`__)
-  ...and more

`Let me know <https://kylegabriel.com/contact/>`__ how you use Mycodo and I may include it on this list.

Screenshots
-----------

Visit the `Screenshots <https://github.com/kizniche/Mycodo/wiki/Screenshots>`__ page of the Wiki.

Install Mycodo
--------------

Prerequisites
~~~~~~~~~~~~~

-  `Raspberry Pi <https://www.raspberrypi.org>`__ single-board computer (any version: Zero, 1, 2, 3, or 4)
-  `Raspberry Pi Operating System <https://www.raspberrypi.org/downloads/raspberry-pi-os/>`__ flashed to a micro SD card
-  An active internet connection

Mycodo has been tested to work with Raspberry Pi OS Lite (2020-05-27), and also the Desktop version if using Mycodo version => 8.6.0.

Install
~~~~~~~

Once you have the Raspberry Pi booted into the Raspberry Pi OS with an internet connection, run the following command in a terminal to initiate the Mycodo install:

.. code:: bash

    curl -L https://kizniche.github.io/Mycodo/install | bash


Install Notes
~~~~~~~~~~~~~

Make sure the install script finishes without errors. A log of the output will be created at ``~/Mycodo/install/setup.log``.

If the install is successful, the web user interface should be accessible by navigating a web browser to ``https://127.0.0.1/``, replacing ``127.0.0.1`` with your Raspberry Pi's IP address. Upon your first visit, you will be prompted to create an admin user before being redirected to the login page. Once logged in, check that the time is correct at the top left of the page. Incorrect time can cause a number of issues with measurement storage and retrieval, among others. Also ensure the host name and version number at the top left of the page is green, indicating the daemon is running. Red indicates the daemon is inactive or unresponsive. Last, ensure any java-blocking plugins of your browser are disabled for all parts of the web interface to function properly.

If you receive an error during the install that you believe is preventing your system from operating, please `create an issue <https://github.com/kizniche/Mycodo/issues>`__ with the install log attached. If you would first like to attempt to diagnose the issue yourself, see `Diagnosing Issues <#diagnosing-issues>`__.

A minimal set of anonymous usage statistics are collected to help improve development. No identifying information is saved from the information that is collected and it is only used to improve Mycodo. No other sources will have access to this information. The data collected is mainly what and how many features are used, and other similar information. The data that's collected can be viewed from the 'View collected statistics' link in the ``Settings -> General`` page. There is an opt out option on the General Settings page.

REST API
--------

The latest API documentation can be found here: `API Information <https://kizniche.github.io/Mycodo/API/>`__ and `API Endpoint Documentation <https://kizniche.github.io/Mycodo/mycodo-api.html>`__.

About PID Control
-----------------

A `proportional???integral???derivative (PID) controller <https://en.wikipedia.org/wiki/PID_controller>`__ is a control loop feedback mechanism used throughout industry for controlling systems. It efficiently brings a measurable condition, such as temperature, to a desired state (setpoint). A well-tuned PID controller can raise to a setpoint quickly, have minimal overshoot, and maintain the setpoint with little oscillation.

.. figure:: docs/images/PID-Animation.gif
   :alt: PID Animation


|Mycodo|

The top graph visualizes the regulation of temperature. The red line is the desired temperature (setpoint) that has been configured to change over the course of each day. The blue line is the actual recorded temperature. The green vertical bars represent how long a heater has been activated for every 20-second period. This regulation was achieved with minimal tuning, and already displays a very minimal deviation from the setpoint (??0.5?? Celsius). Further tuning would reduce this variability further.

See the `PID Controller <https://kizniche.github.io/Mycodo/Functions/#pid-controller>`__ and `PID Tuning <https://kizniche.github.io/Mycodo/Functions/#pid-tuning>`__ sections of the manual for more information.

Supported Inputs and Outputs
----------------------------

All supported Inputs, Outputs, and other devices can be found under the `Supported Devices <https://kizniche.github.io/Mycodo/Supported-Inputs-By-Measurement/>`__ section of the manual.

Custom Inputs, Outputs, and Controllers
---------------------------------------

Mycodo supports importing custom Input, Output, and Controller modules. you can find more information about each in the manual under `Custom Inputs <https://kizniche.github.io/Mycodo/Inputs/#custom-inputs>`__, `Custom Outputs <https://kizniche.github.io/Mycodo/Outputs/#custom-outputs>`__, and `Custom Functions <https://kizniche.github.io/Mycodo/Functions/#custom-functions>`__.

If you would like to add to the list of supported Inputs, Outputs, and Controllers, submit a pull request with the module you created or start a `New Issue <https://github.com/kizniche/Mycodo/issues/new?assignees=&labels=&template=feature-request.md&title=>`__.

Additionally, I have another github repository devoted to custom Inputs, Outputs, and Controllers that do not necessarily fit with the built-in set and are not included by default with Mycodo, but can be imported. These can be found at `kizniche/Mycodo-custom <https://github.com/kizniche/Mycodo-custom>`__.

Links
-----

Thanks for using and supporting Mycodo, however depending where you found this documentation, you may not have the latest version or it may have been altered, if not obtained through an official distribution site. You should be able to find the latest version on github or my web site at the following links.

https://github.com/kizniche/Mycodo

https://KyleGabriel.com

License
-------

See `License.txt <https://github.com/kizniche/Mycodo/blob/master/LICENSE.txt>`__

Mycodo is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

Mycodo is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the `GNU General Public License <http://www.gnu.org/licenses/gpl-3.0.en.html>`__ for more details.

A full copy of the GNU General Public License can be found at http://www.gnu.org/licenses/gpl-3.0.en.html

This software includes third party open source software components. Please see individual files for license information, if applicable.

Languages
---------

|Translation Table|

-  Native: English
-  `Dutch <#dutch>`__,
   `German <#german>`__,
   `French <#french>`__,
   `Italian <#italian>`__,
   `Norwegian <#norwegian>`__,
   `Polish <#polish>`__,
   `Portuguese <#portuguese>`__,
   `Russian <#russian>`__,
   `Serbian <#serbian>`__,
   `Spanish <#spanish>`__,
   `Swedish <#swedish>`__,
   `Chinese <#chinese>`__.

By default, mycodo will display the default language set by your browser. You may also force a language in the settings at ``[Gear Icon] -> Configure -> General -> Language``

If you would like to improve the translations, you can make changes at `http://translate.kylegabriel.com <http://translate.kylegabriel.com:8080/engage/mycodo/>`__, submit a pull request with an amended .po file from ~/Mycodo/mycodo/mycodo_flask/translations/, or start a `New Issue <https://github.com/kizniche/Mycodo/issues/new>`__ detailing the corrections.

English
~~~~~~~

The native language used in the software.

Dutch
~~~~~

Mycodo is een geautomatiseerd monitoring- en regelsysteem dat is gebouwd
om op de Raspberry Pi te draaien (versies Zero, 1, 2, 3 en 4).

Oorspronkelijk ontworpen om eetbare paddenstoelen te kweken, is Mycodo
uitgegroeid tot het vermogen om veel meer te doen, waaronder het kweken
van planten, het kweken van micro-organismen, het onderhouden van
bijenbijen bij de bijen, het incuberen van dieren en eieren, het
onderhouden van aquatische systemen, het ouder worden van kazen, het
fermenteren van voedsel en tabak, het koken eten (sous-vide) en meer.

Het systeem bestaat uit een backend (daemon) en een frontend
(gebruikersinterface). De backend voert metingen uit van sensoren en
apparaten, co??rdineert vervolgens een diverse reeks antwoorden op die
metingen, inclusief het vermogen om outputs te moduleren (relais, PWM,
draadloze outlets), omgevingsomstandigheden te regelen met elektrische
apparaten onder PID-regeling (gestage regeling of omschakeling tijd),
timers plannen, foto's maken en video streamen, acties activeren wanneer
metingen aan bepaalde voorwaarden voldoen (relais moduleren, opdrachten
uitvoeren, per e-mail op de hoogte stellen, etc.) en meer. De frontend is
een webinterface die gemakkelijke navigatie en configuratie mogelijk
maakt vanaf elk apparaat met een browser.

French
~~~~~~

Mycodo est un syst??me de surveillance et de r??gulation automatis?? con??u
pour fonctionner sur le Raspberry Pi (versions z??ro, 1, 2, 3 et 4).

Con??u ?? l'origine pour cultiver des champignons comestibles, Mycodo s'est
d??velopp?? pour inclure la capacit?? de faire beaucoup plus, notamment la
culture de plantes, la culture de micro-organismes, le maintien de
l'hom??ostasie du rucher des abeilles, la mise en incubation des animaux
et des ??ufs, la maintenance des syst??mes aquatiques, le vieillissement
des fromages, la fermentation nourriture (sous vide), et plus.

Le syst??me comprend un serveur (d??mon) et une interface utilisateur
(interface utilisateur). Le syst??me effectue des mesures ?? partir de
capteurs et d???appareils, puis coordonne un ensemble divers de r??ponses ??
ces mesures, notamment la possibilit?? de moduler les sorties (relais,
PWM, prises sans fil), de r??guler les conditions environnementales avec
des appareils ??lectriques sous contr??le PID (r??gulation continue ou
basculement temps), planifiez des minuteries, capturez des photos et des
flux vid??o, d??clenchez des actions lorsque les mesures r??pondent ??
certaines conditions (moduler des relais, ex??cuter des commandes, notifier
par courrier ??lectronique, etc.), etc. L'interface Web est une interface
Web qui facilite la navigation et la configuration ?? partir de tout
appareil compatible avec le navigateur.

German
~~~~~~

Mycodo ist ein automatisiertes ??berwachungs- und Regulierungssystem, das
f??r den Raspberry Pi (Versionen Zero, 1, 2, 3 und 4) entwickelt wurde.

Urspr??nglich f??r die Kultivierung von Speisepilzen konzipiert, hat Mycodo
die F??higkeit zu weitaus mehr erweitert, darunter die Kultivierung von
Pflanzen, die Kultivierung von Mikroorganismen, die Aufrechterhaltung der
Hom??ostase der Bienenhaus-Bienenh??user, die Inkubation von Tieren und
Eiern, die Aufrechterhaltung von Wassersystemen, das Altern von K??se, das
G??ren von Lebensmitteln und Tabak sowie das Kochen Essen (Sous-Vide) und
mehr.

Das System besteht aus einem Backend (Daemon) und einem Frontend
(Benutzeroberfl??che). Das Backend f??hrt Messungen von Sensoren und Ger??ten
durch und koordiniert dann eine Vielzahl von Reaktionen auf diese
Messungen, einschlie??lich der M??glichkeit, Ausg??nge (Relais, PWM,
drahtlose Ausg??nge) zu modulieren und Umgebungsbedingungen mit elektrischen
Ger??ten unter PID-Steuerung zu regulieren (stetige Regelung oder
Umschaltung) Zeit), Zeitpl??ne planen, Fotos aufnehmen und Videos streamen,
Aktionen ausl??sen, wenn Messungen bestimmte Bedingungen erf??llen (Relais
modulieren, Befehle ausf??hren, per E-Mail benachrichtigen usw.) und vieles
mehr. Das Frontend ist eine Weboberfl??che, die eine einfache Navigation und
Konfiguration von jedem Browser-f??higen Ger??t aus erm??glicht.

Italian
~~~~~~~

Mycodo ?? un sistema di monitoraggio e regolazione automatico che ?? stato
creato per funzionare sul Raspberry Pi (versioni Zero, 1, 2, 3 e 4).

Originariamente progettato per coltivare funghi commestibili, Mycodo ??
cresciuto fino a comprendere la capacit?? di fare molto di pi??, coltivando
piante, coltivando microrganismi, mantenendo l'omeostasi delle api apistiche
del miele, incubando animali e uova, mantenendo sistemi acquatici, formaggi
stagionati, alimenti fermentati e tabacco, cucinando cibo (sous-vide) e
altro ancora.

Il sistema comprende un backend (demone) e un frontend (interfaccia utente).
Il back-end esegue misurazioni da sensori e dispositivi, quindi coordina un
insieme diversificato di risposte a tali misurazioni, inclusa la possibilit??
di modulare le uscite (rel??, PWM, prese wireless), regola le condizioni
ambientali con dispositivi elettrici sotto controllo PID (regolazione costante
o commutazione tempo), programmare i timer, acquisire foto e trasmettere
video, attivare azioni quando le misurazioni soddisfano determinate condizioni
(modulazione di rel??, esecuzione di comandi, notifica via e-mail, ecc.) e
altro. Il frontend ?? un'interfaccia web che consente una facile navigazione e
configurazione da qualsiasi dispositivo abilitato per il browser.

Norwegian
~~~~~~~~~

Mycodo er et automatisert overv??kings- og reguleringssystem som ble bygget
for ?? kj??re p?? Raspberry Pi (versjoner Zero, 1, 2, 3 og 4).

Mycodo er opprinnelig utviklet for ?? dyrke spiselige sopp, og har vokst
til ?? inkludere muligheten til ?? gj??re mye mer, inkludert dyrking av
planter, dyrking av mikroorganismer, opprettholder honningbi apiary
homeostasis, inkubering av dyr og egg, opprettholde akvatiske systemer,
aldrende oster, fermenterende matvarer og tobakk, matlaging mat (sous-vide)
og mer.

Systemet best??r av en backend (daemon) og en frontend (brukergrensesnitt).
Backend utf??rer m??linger fra sensorer og enheter, og koordinerer deretter
et mangfoldig sett med svar p?? disse m??lingene, inkludert muligheten til ??
modulere utganger (rel??er, PWM, tr??dl??se uttak), regulere milj??forhold med
elektriske enheter under PID-kontroll (stabil regulering eller endring over
tid), planlegge timere, ta bilder og streame video, utl??se handlinger n??r
m??lingene oppfyller visse forhold (modulere rel??er, utf??re kommandoer,
varsle via e-post, etc.) og mer. Frontend er et webgrensesnitt som gj??r det
enkelt ?? navigere og konfigurere fra hvilken som helst nettleseraktivert
enhet.

Polish
~~~~~~

Mycodo to zautomatyzowany system monitorowania i regulacji, kt??ry zosta?? zbudowany do pracy na Raspberry Pi (wersje Zero, 1, 2 i 3).

Pierwotnie zaprojektowany do uprawy grzyb??w jadalnych, Mycodo rozwin????o si??, aby umo??liwi?? znacznie wi??cej, w tym upraw?? ro??lin, hodowl?? mikroorganizm??w, utrzymanie homeostazy pszcz???? miodnych, inkubacj?? zwierz??t i jaj, utrzymanie system??w wodnych, dojrzewanie ser??w, fermentacj?? ??ywno??ci i tytoniu, gotowanie jedzenie (sous-vide) i nie tylko.

System sk??ada si?? z zaplecza (demona) i frontendu (interfejsu u??ytkownika). Backend przeprowadza pomiary z czujnik??w i urz??dze??, a nast??pnie koordynuje zr????nicowany zestaw odpowiedzi na te pomiary, w tym mo??liwo???? modulacji wyj???? (przeka??niki, PWM, wyj??cia bezprzewodowe), regulacj?? warunk??w ??rodowiskowych za pomoc?? urz??dze?? elektrycznych pod kontrol?? PID (regulacja sta??a lub prze????czanie czas), ustawianie timer??w, robienie zdj???? i strumieniowanie wideo, wyzwalanie dzia??a??, gdy pomiary spe??niaj?? okre??lone warunki (modulacja przeka??nik??w, wykonywanie polece??, powiadamianie przez e-mail itp.) i nie tylko. Frontend to interfejs sieciowy, kt??ry umo??liwia ??atw?? nawigacj?? i konfiguracj?? z dowolnego urz??dzenia obs??uguj??cego przegl??dark??.

Portuguese
~~~~~~~~~~

O Mycodo ?? um sistema automatizado de monitoramento e regula????o que foi
constru??do para rodar no Raspberry Pi (vers??es Zero, 1, 2, 3 e 4).

Originalmente concebido para cultivar cogumelos comest??veis, o Mycodo
cresceu para incluir a capacidade de fazer muito mais, incluindo cultivar
plantas, cultivar microorganismos, manter a homeostase do api??rio de
abelhas, incubar animais e ovos, manter sistemas aqu??ticos, queijos
envelhecidos, fermentar alimentos e tabaco, cozinhar comida (sous-vide) e
muito mais.

O sistema compreende um backend (daemon) e um frontend (interface de
usu??rio). O backend conduz medi????es a partir de sensores e dispositivos e
coordena um conjunto diversificado de respostas a essas medi????es,
incluindo a capacidade de modular sa??das (rel??s, PWM, tomadas sem fio),
regular as condi????es ambientais com dispositivos el??tricos sob controle
PID (regula????o est??vel ou troca tempo), agendar cron??metros, capturar
fotos e transmitir v??deo, acionar a????es quando as medi????es atenderem a
determinadas condi????es (modular rel??s, executar comandos, notificar por
e-mail etc.) e muito mais. O frontend ?? uma interface da web que permite
f??cil navega????o e configura????o a partir de qualquer dispositivo habilitado
para navegador.

Russian
~~~~~~~

Mycodo - ?????? ???????????????????????????????????? ?????????????? ?????????????????????? ?? ??????????????????????????,
?????????????????? ?????? ???????????? ???? Raspberry Pi (???????????? Zero, 1, 2, 3 ?? 4).

?????????????????????????? ?????????????????????????? ?????? ?????????????????????? ?????????????????? ????????????, Mycodo
?????????? ?? ???????????? ???????????????? ???????????? ?????????????? ????????????, ?????????????? ??????????????????????
????????????????, ?????????????????????? ??????????????????????????????, ?????????????????????? ???????????????????? ????????????
???????????????????? ????????, ?????????????????? ???????????????? ?? ??????, ?????????????????????? ???????????? ????????????,
???????????????? ??????????, ?????????????????????? ?????????????????? ?? ????????????, ?????????????????????????? ????????. ??????
(sous-vide) ?? ???????????? ????????????.

?????????????? ???????????????? ?? ???????? ???????????? (??????????) ?? ?????????????????? (????????????????????????????????
??????????????????). ???????????? ???????????????? ?????????????????? ???? ???????????????? ?? ??????????????????, ??????????
???????????????????????? ?????????????????????????? ?????????? ?????????????? ???? ?????? ??????????????????, ??????????????
?????????????????????? ???????????????????????? ???????????? (????????, ??????, ???????????????????????? ????????????),
???????????????????????? ?????????????? ???????????????????? ?????????? ?? ?????????????? ?????????????????????????? ??????????????????
?????? ?????????????????????? ?????? (???????????????????? ?????????????????????????? ?????? ????????????????????????). ??????????),
?????????????????????? ??????????????, ?????????????????????? ???????????????????? ?? ?????????????????? ??????????, ??????????????????
????????????????, ?????????? ?????????????????? ?????????????????????????? ???????????????????????? ????????????????
(???????????????????????? ????????, ?????????????????? ??????????????, ???????????????????? ?????????????????????? ????
?????????????????????? ?????????? ?? ??. ??.) ?? ???????????? ????????????. ?????????????????? ???????????????????????? ??????????
??????-??????????????????, ?????????????? ???????????????????????? ?????????????? ?????????????????? ?? ?????????????????? ?? ????????????
???????????????????? ?? ???????????????????? ????????????????.

Serbian
~~~~~~~

???????????? ???? ???????????????????? ???????????? ???? ???????????? ?? ???????????????????? ???????? ???? ?????????????????? ????
???????? ???? ?????????????????? ???? (?????????????? ????????, 1, 2, 3 ?? 4).

???????????????????? ???????????????????? ???? ???????????????? ???????????????? ??????????, ???????????? ???? ???????????????? ????
?????????????????? ???? ?????????? ?????????? ????????, ???????????????????? ?????????????????????? ????????????, ??????????????????????
??????????????????????????????, ?????????????????? ???????????????????? ???????????????? ????????, ???????????????????? ????????????????
?? ????????, ?????????????????? ?????????????? ??????????????, ?????????????? ????????????, ???????????????????????? ?????????? ??
??????????, ???????????? ?????????? (????????-????????), ?? ????????.

???????????? ???????????? ?????????????? (????????????) ?? ???????????????? (???????????????????? ??????????????????). ??????????????
???????? ???????????? ???? ?????????????? ?? ??????????????, ?????????? ???????????????????? ?????????????????? ???????????????? ????
???? ????????????, ???????????????????? ?????????????????? ???????????????????? ???????????? (????????????, ??????, ??????????????
????????????????), ???????????????????? ???????????? ?????????????? ???? ?????????????????????? ?????????????????? ?????? ??????
?????????????????? (???????????? ???????????????????? ?????? ?????????????? ??????????), ???????????????? ??????????????, ??????????????
?????????????????????? ?? ???????????????????? ?????????? ??????????????, ???????????? ?????????????????? ???????? ????????????
???????????????????? ???????????????? ???????????? (???????????????????? ????????????, ???????????????????? ??????????????,
???????????????????????? ?????????? ??-??????????, ??????.), ?? ?????? ?????????? ????????. ???????????????? ???? ??????
?????????????????? ???????? ?????????????????? ?????????????????????? ???????????????????? ?? ?????????????????????????? ???? ????????
?????? ?????????????? ???? ???????????????????? ??????????????????????????.

Spanish
~~~~~~~

Mycodo es un sistema automatizado de monitoreo y regulaci??n que fue creado
para ejecutarse en la Raspberry Pi (versiones cero, 1, 2, 3 y 4).

Originalmente dise??ado para cultivar hongos comestibles, Mycodo ha crecido
para incluir la capacidad de hacer mucho m??s, incluido el cultivo de plantas,
el cultivo de microorganismos, el mantenimiento de la homeostasis de las
abejas, la incubaci??n de animales y huevos, el mantenimiento de los sistemas
acu??ticos, el envejecimiento de los quesos, la fermentaci??n de alimentos y el
tabaco, la cocina. comida (sous-vide), y m??s.

El sistema comprende un backend (daemon) y un frontend (interfaz de usuario).
El backend realiza mediciones desde sensores y dispositivos, luego coordina
un conjunto diverso de respuestas a esas mediciones, incluida la capacidad
de modular salidas (rel??s, PWM, salidas inal??mbricas), regular las
condiciones ambientales con dispositivos el??ctricos bajo control PID
(regulaci??n constante o cambio tiempo), programe temporizadores, capture
fotos y transmita videos, active acciones cuando las mediciones cumplan
ciertas condiciones (module rel??s, ejecute comandos, notifique por correo
electr??nico, etc.) y m??s. La interfaz es una interfaz web que permite una
f??cil navegaci??n y configuraci??n desde cualquier dispositivo con navegador.

Swedish
~~~~~~~

Mycodo ??r ett automatiserat ??vervaknings- och reglersystem som byggdes
f??r att springa p?? Raspberry Pi (versioner noll, 1, 2, 3 och 4).

Mycodo har ursprungligen utformats f??r att odla ??tliga svampar, och har
d??rmed ??kat m??jligheten att g??ra mycket mer, inklusive odling av v??xter,
odlingsmikroorganismer, uppr??tth??llande av honeybee apiary homeostasis,
inkubering av djur och ??gg, uppr??tth??llande av vattenlevande system,
??ldrande ostar, j??sning av mat och tobak, matlagning mat (sous-vide)
och mer.

Systemet innefattar en backend (daemon) och en frontend
(anv??ndargr??nssnitt). Bakgrunden utf??r m??tningar fr??n sensorer och
enheter och samordnar sedan en m??ngd olika svar p?? dessa m??tningar,
inklusive m??jligheten att modulera utg??ngar (rel??er, PWM, tr??dl??sa
uttag), reglera milj??f??rh??llandena med elektriska enheter under
PID-kontroll (st??ndig reglering eller byte ??ver tid), schemal??gg timer,
ta bilder och str??mma video, utl??s ??tg??rder n??r m??tningar uppfyller
vissa villkor (modulera rel??er, utf??ra kommandon, meddela via e-post
etc.) och mer. Frontend ??r ett webbgr??nssnitt som m??jligg??r enkel
navigering och konfiguration fr??n alla webbl??saraktiverade enheter.

Chinese
~~~~~~~

Mycodo?????????????????????????????????????????????Raspberry Pi?????????????????????Zero???1,2,3???4??????

Mycodo????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????sous-vide????????????

?????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????PWM????????????????????????????????????PID????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????????Web????????????????????????????????????????????????????????????????????????


.. |Build Status| image:: https://github.com/kizniche/Mycodo/actions/workflows/main.yml/badge.svg
   :target: https://github.com/kizniche/Mycodo/actions/workflows/main.yml
.. |Codacy Badge| image:: https://app.codacy.com/project/badge/Grade/bb5ffc43e4444231b813ca6e81359336
   :target: https://www.codacy.com/gh/kizniche/Mycodo/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=kizniche/Mycodo&amp;utm_campaign=Badge_Grade
.. |Translation Badge| image:: http://translate.kylegabriel.com:8080/widgets/mycodo/-/svg-badge.svg
   :target: http://translate.kylegabriel.com:8080/engage/mycodo/
.. |Translation Table| image:: http://translate.kylegabriel.com:8080/widgets/mycodo/-/multi-auto.svg
   :target: http://translate.kylegabriel.com:8080/engage/mycodo/
.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.824199.svg
   :target: https://doi.org/10.5281/zenodo.824199
.. |Mycodo| image:: https://kylegabriel.com/projects/wp-content/uploads/sites/3/2016/05/Mycodo-3.6.0-tango-Graph-2016-05-21-11-15-26.png
   :target: https://kylegabriel.com/projects/

Thanks
------

-  `Alembic <https://alembic.sqlalchemy.org>`__
-  `Argparse <https://pypi.org/project/argparse>`__
-  `Bcrypt <https://pypi.org/project/bcrypt>`__
-  `Bootstrap <https://getbootstrap.com>`__
-  `Daemonize <https://pypi.org/project/daemonize>`__
-  `Date Range Picker <https://github.com/dangrossman/daterangepicker>`__
-  `Distro <https://pypi.org/project/distro>`__
-  `Email_Validator <https://pypi.org/project/email_validator>`__
-  `Filelock <https://pypi.org/project/filelock>`__
-  `Flask <https://pypi.org/project/flask>`__
-  `Flask_Accept <https://pypi.org/project/flask_accept>`__
-  `Flask_Babel <https://pypi.org/project/flask_babel>`__
-  `Flask_Compress <https://pypi.org/project/flask_compress>`__
-  `Flask_Limiter <https://pypi.org/project/flask_limiter>`__
-  `Flask_Login <https://pypi.org/project/flask_login>`__
-  `Flask_Marshmallow <https://pypi.org/project/flask_marshmallow>`__
-  `Flask_RESTX <https://pypi.org/project/flask_restx>`__
-  `Flask_Session <https://pypi.org/project/flask_session>`__
-  `Flask_SQLAlchemy <https://pypi.org/project/flask_sqlalchemy>`__
-  `Flask_Talisman <https://pypi.org/project/flask_talisman>`__
-  `Flask_WTF <https://pypi.org/project/flask_wtf>`__
-  `FontAwesome <https://fontawesome.com>`__
-  `Geocoder <https://pypi.org/project/geocoder>`__
-  `gridstack.js <https://github.com/gridstack/gridstack.js>`__
-  `Gunicorn <https://gunicorn.org>`__
-  `Highcharts <https://www.highcharts.com>`__
-  `InfluxDB <https://github.com/influxdata/influxdb>`__
-  `jQuery <https://jquery.com>`__
-  `Marshmallow_SQLAlchemy <https://pypi.org/project/marshmallow_sqlalchemy>`__
-  `Pyro5 <https://github.com/irmen/Pyro5>`__
-  `SQLAlchemy <https://www.sqlalchemy.org>`__
-  `SQLite <https://www.sqlite.org>`__
-  `toastr <https://github.com/CodeSeven/toastr>`__
-  `WTForms <https://pypi.org/project/wtforms>`__

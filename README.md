# verbraucherpreise

![Dashboard über die Entwicklung der Verbraucherpreise](https://github.com/Burak-Oezkan/verbraucherpreise/blob/main/Verbraucherpreise/Bilder/4-1-Dashboard.png)
1. Untersuchung der Verbraucherpreise 2023:
    * Data Cleaning in PowerQuery und Python 
    * Exploratory Data Analysis (EDA) in PowerBI
    * Erstellung des Dashboards in PowerBI

    * Data Cleaning und EDA: ['Verbraucherpreise/0-Verbraucherpreise.ipynb'](https://github.com/Burak-Oezkan/verbraucherpreise/blob/9589d97655a743d6ebdd10cf63357eb441ff02b4/Verbraucherpreise/0-Verbraucherpreise.ipynb)
    * Dashboard:
        * Power BI Datei: ['Projekt-Verbraucherpreis.pbix'](https://github.com/Burak-Oezkan/verbraucherpreise/blob/9589d97655a743d6ebdd10cf63357eb441ff02b4/Verbraucherpreise/Projekt-Verbraucherpreis.pbix)
        * Vorstellung in PowerPoint: [['Vorstellung-Dashboard.pptx'](https://github.com/Burak-Oezkan/verbraucherpreise/blob/9589d97655a743d6ebdd10cf63357eb441ff02b4/Verbraucherpreise/Vorstellung-Dashboard.pptx)](https://github.com/Burak-Oezkan/verbraucherpreise/blob/9589d97655a743d6ebdd10cf63357eb441ff02b4/Verbraucherpreise/Projekt-Verbraucherpreis.pdf)
        * Vorschau als PDF: ['Projekt-Verbraucherpreis.pdf'](https://github.com/Burak-Oezkan/verbraucherpreise/blob/9589d97655a743d6ebdd10cf63357eb441ff02b4/Verbraucherpreise/Vorstellung-Dashboard.pptx)

## Übersicht

Die Verbraucherpreise sind während der Pandemie und insbesondere nach dem Krieg in der Ukraine stark gestiegen. Die Preisentwicklung ist ein sehr wichtiger Indikator für die Analyse einer Volkswirtschaft und dient als grundlegendes Instrument für die politische Entscheidungsfindung.  
Zur Messung der Preisentwicklung werden der **Verbraucherpreisindex (VPI)** und der **Erzeugerpreisindex (EPI)** des Statistischen Bundesamtes verwendet.  
Bei der Entwicklung der Indizes wird ein **Basisjahr** festgelegt, das in regelmäßigen Abständen durch ein neues Basisjahr ersetzt wird. Die Werte für das Basisjahr sind immer 100 und die restlichen Werte bauen auf diesem Wert auf.  

> "In der **Preisstatistik** werden Ergebnisse von **zeitlichen Preisvergleichen** in Form von **Indizes** monatlich beziehungsweise vierteljährlich veröffentlicht. Das deutsche preisstatistische System folgt dabei in seinem Aufbau den Stufen, die Güter auf ihrem Weg vom Import oder von der Produktion bis zum Endverbrauch durchlaufen können."  

[Quelle](https://www.destatis.de/DE/Themen/Wirtschaft/Preise/Ueberblick/einfuehrung.html?nn=467346)

**Verbraucherpreisindex (VPI)**:  
> "Der Verbraucherpreisindex misst monatlich die durchschnittliche Preisentwicklung aller Waren und Dienstleistungen, die private Haushalte in Deutschland für Konsumzwecke kaufen. Die Veränderung des Verbraucherpreisindex zum Vorjahresmonat bzw. zum Vorjahr wird als Teuerungsrate oder als Inflationsrate bezeichnet.
Beim Berechnen des Verbraucherpreisindex bzw. der Inflationsrate verwenden wir einen "Warenkorb", der rund 700 Güterarten umfasst und sämtliche von privaten Haushalten in Deutschland gekauften Waren und Dienstleistungen repräsentiert. Mit welchen Gewichten diese Güterarten in den Gesamtindex einfließen, ist im Wägungsschema festgehalten."

[Quelle](https://www.destatis.de/DE/Themen/Wirtschaft/Preise/Verbraucherpreisindex/_inhalt.html)

**Erzeugerpreisindex gewerblicher Produkte (EPI)**:

>"Der vom Statistischen Bundesamt monatlich ermittelte Erzeugerpreisindex gewerblicher Produkte misst die durchschnittliche Preisentwicklung von Rohstoffen und Industrieerzeugnissen, die von inländischen Unternehmen abgebaut bzw. hergestellt und im Inland verkauft werden. Die Produzenten dieser Güter gehören zu den Wirtschaftszweigen des Bergbaus und der Gewinnung von Steinen und Erden, des Verarbeitenden Gewerbes und der Energie- und Wasserversorgung."

[Quelle](https://www.bundesbank.de/de/statistiken/konjunktur-und-preise/erzeuger-und-verbraucherpreise/erzeuger-und-verbraucherpreise-775284)

**Inflationsrate:**

Die Inflationsrate ist ein Maß für die prozentuale Veränderung der Preisindizes gegenüber dem Vorjahr. Ist sie rückläufig, spricht man von **Deflation**.

**Weitere Informationen:**:

* https://www.destatis.de/DE/Themen/Wirtschaft/Preise/Ueberblick/_inhalt.html
* https://www.bundesbank.de/de/statistiken/konjunktur-und-preise/erzeuger-und-verbraucherpreise/erzeuger-und-verbraucherpreise-775284

Wir wollen genauer untersuchen, wie sich der Verbraucher- und der Erzeugerpreisindex in den letzten Jahren entwickelt haben.  

**Mögliche Fragen:**:

1. Wie stark sind die Preise gestiegen?
2. Wann sind die Preise gestiegen?
3. Welche Produkte sind besonders betroffen?
4. Ist der Anstieg an Verbraucherpreisen und Erzeugerpreisen proportional?

**Daten**:

Alle Daten, die wir verwenden werden, sind auf der Website des Statistischen Bundesamtes zu finden. Es werden jeweils die Daten der Jahre 2018 bis 2023 berücksichtigt.

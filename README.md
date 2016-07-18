# Startpunkte / Vorlagen
http://github.com/marcusvetter/yoda-chat
http://github.com/christianeder/angular2-webpack-aspnetcore

# Packagemanagement
- **npm** (reicht unserer Meinung nach vollkommen aus)
- Alternativ/Ergänzend:
    - bower
    - jspm

# Build
- **Webpack**
    - Vereinfacht Tasks, die man in der SPA-Entwicklung oft benötigt (z.B. Kompilieren von TypeScript)
    - Schaut auf Änderungen im Code und lädt Anwendung automatisch neu
    - Tasks könnten auch mit Gulp/Grunt erstellt werden, ist aber aufwändiger
- Alternativ:
    - Gulp (moderner als Grunt, funktionsbasiert)
    - Grunt (konfigurationsbasiert)

# Entwicklungssprachen
- Skriptsprachen
    - **TypeScript** (Vorteile gegenüber JavaScript: Typsicherheit, dadurch Refactorings, erzwingt mehr Clean Code, enthält ES6 und ES7 Features)
    - JavaScript
- Markup
    - HTML
    - Jade (je nach Geschack, spart einige Klammern, bei komponentenbasiertem Framework wie z.B. Angular2 teilw. überflüssige Features)
- Styling
    - CSS (bei Verwendung von Angular2 und klein geschnittenen Komponenten ausreichend abgesehen von nicht unterstützen Variablen)
    - SASS vs LESS je nach Geschmack
    - Webpack macht Verwendung extrem einfach - sogar für einzelne Komponenten
    - **Wiederverwendbare Styles (Mixins, Variablen)** vs gestylte Komponenten / Layout-Komponenten

# Frameworks für Web-Anwendung (SPA)
- Angular1 (Sehr etabliertes Framework, große Community, ggf. Performanzeinschränkungen bei sehr großen Daten)
- Angular2 (Framework, Momentan noch RC4, leider bisher häufig Breaking Changes)
- Aurelia (Framework, scheint vielversprechend zu sein, leider bisher noch keine praktische Erfahrung)
- ReactJS (Library, kein Framework. Leider bisher noch keine praktische Erfahrung)

# Frameworks für Unit-Test
- Runner-Framework
    - **Karma** (de-facto Standard)
    - Chutzpah
    - Mocha
- Assertion-Framework
    - **Jasmine**
    - Chai / ChaiAsPromised / Sinon (alternativ, oder z.B. für Akzeptanztests)

# Frameworks für Akzeptanztests
- **Protractor** (empfohlen von Angular/Aurelia)
- WebdriverJS (Protractor erweitert WebdriveJS-API)
- **Cucumber** (Akzeptanzgetriebenes Testen)

# Allgemein
- Keine internal Modules verwenden! => Läuft nur mit Webpack/Browserify/... im Browser (da historisch konzipiert für Node)
- Clean Code bei SPAs extrem wichtig :-)
- Komponentenbasiert entwicklen! (Eine Komponente besteht aus Businesslogik, DOM, Styles, Assets, Tests)

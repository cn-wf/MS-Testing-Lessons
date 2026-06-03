# Testfallentwurf Market Mate

**Entwirf deine Testfälle auf Grundlage der Funktionen, die für das nächste Release der sozialen Medienplattform entwickelt werden sollen!**

**Du musst sie nur *entwerfen* – die Testdurchführung erfolgt in einer späteren Phase.**

**Füge, falls zutreffend, das verwendete Testentwurfsverfahren hinzu.**

Beispielsoftware: Market Mate *[(*https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/))

---

### **1. Bewertungssystem für Produkte**

**Testentwurfsverfahren**: Anwendungsfalltest (Use Case Testing), Äquivalenzklassenbildung (EP), Fehlerermessen (Error Guessing)

### Testfälle:

1. **Fehlerermessen**:
    - **Testfall**: Überprüfen des Systemverhaltens, wenn eine Beschreibung aber kein Rating angegeben wird
        - **Eingabe**: Sternerating bleibt leer. Beschreibungsfeld = “Beschreibung”.
        - **Erwartetes Ergebnis**: Fehlermeldung “Rating fehlt”
2. **Äquivalenzklassenbildung**:
    - **Testfall**: Überprüfen des Systemverhaltens bei vorhandenem Rating ohne Beschreibung.
        - **Eingabe**: Beschreibung bleibt leer. Sternerating = 4 Sterne
        - **Erwartetes Ergebnis**: Bewertung erfolgreich abgegeben.
3. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen des Systemverhaltens, beim Versuch eine zweite Bewertung abzugeben, während die erste existiert.
        - **Eingabe**: Navigation zur Bewertung eines bereits bewerteten Artikels.
        - **Erwartetes Ergebnis**: Bewertungsfenster erscheint nicht.
4. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen des Systemverhaltens, beim Versuch eine zweite Bewertung abzugeben, nachdem die erste gelöscht wurde.
        - **Eingabe**: Navigation zur Bewertung eines bereits bewerteten Artikels, bei dem die erste Bewertung gelöscht wurde.
        - **Erwartetes Ergebnis**: Bewertung kann abgegeben werden.

### **2. Altersverifikation für alkoholische Produkte**

**Testentwurfsverfahren**: Anwendungsfalltest (Use Case Testing), Grenzwertanalyse (BVA)

### Testfälle:

1. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen des Systemverhaltens, nach geschlossenem Altersverifikationfenster.
        - **Eingabe**: Schließen der Altersabfrage ohne Eingabe.
        - **Erwartetes Ergebnis**: “Alcohol” Kategorie kann nicht eingesehen werden.
2. **Grenzwertanalyse**:
    - **Testfall**: Überprüfen einer Alterseingabe von unter 18 Jahren.
        - **Eingabe**: Alter = Heute - 17 Jahre
        - **Erwartetes Ergebnis**: “Alcohol” Kategorie kann nicht eingesehen werden.
3. Grenzwertanalyse:
    - **Testfall**: Überprüfen einer Alterseingabe von genau 18 Jahren.
        - **Eingabe**: Alter = Heute - 18 Jahre
        - **Erwartetes Ergebnis**: “Alcohol” Kategorie kann eingesehen werden.
4. Grenzwertanalyse::
    - **Testfall**: Überprüfen einer Alterseingabe von über 18 Jahren.
        - **Eingabe**: Alter = Heute - 19 Jahre
        - **Erwartetes Ergebnis**: “Alcohol” Kategorie kann eingesehen werden.
5. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen, ob die Altersanfrage beim öffnen der Kategorie “Alkohol” auftritt oder beim betreten des Shops
        - **Eingabe**: Navigation zum Shopreiter. Navigation zur Kategorie “Alcohol”.
        - **Erwartetes Ergebnis**: Altersverifikation tritt nur bei der ersten Navigation zur Shopseite auf.
6. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen, dass die Kategorien außer “Alkohol” immer sichtbar sind.
        - **Eingabe**: Registrierung als Minderjähriger. Navigation zu “Fish”
        - **Erwartetes Ergebnis**: Kategorie “Fish” kann eingesehen werden.

---

### **3. Änderungen bei den Versandkosten**

**Testentwurfsverfahren**: Grenzwertanalyse (BVA), Äquivalenzklassenbildung (EP), Fehlerermessen (Error Guessing), Anwendungsfalltest (Use Case Testing)

### Testfälle:

1. **Grenzwertanalyse**:
    - **Testfall**: Überprüfen der Versandkosten bei 20 Euro Warenwert.
        - **Eingabe**: Warenkorb mit Waren im Wert von 20 Euro füllen.
        - **Erwartetes Ergebnis**: Versandkosten sind 0 Euro.
2. **Grenzwertanalyse**:
    - **Testfall**: Überprüfen der Versandkosten bei mehr als 20 Euro Warenwert.
        - **Eingabe**: Warenkorb mit Waren im Wert von 25 Euro füllen.
        - **Erwartetes Ergebnis**: Versandkosten sind 0 Euro.
3. **Grenzwertanalyse**:
    - **Testfall**: Überprüfen der Versandkosten bei weniger als 20 Euro Warenwert.
        - **Eingabe**: Warenkorb mit Waren im Wert von 19 Euro füllen.
        - **Erwartetes Ergebnis**: Versandkosten sind 5 Euro.
4. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen der Versandkosten nachdem ein Warenwert von 20 Euro erreicht wurde und anschließend Waren entfernt werden und ein Wert von 20 Euro unterschritten wird.
        - **Eingabe**: Warenkorb mit Waren im Wert von 25 Euro füllen. Anschließend Waren im Wert von 10 Euro entfernen.
        - **Erwartetes Ergebnis**: Sobald ein Warenwert von 20 Euro unterschritten wird, werden die Versandkosten wieder hinzugefügt.
5. **Anwendungsfalltest**:
    - **Testfall**: Überprüfen der Versandkosten nachdem der Warenkorb befüllt und wieder entleert wurde.
        - **Eingabe**: Warenkorb mit Waren im Wert von 25 Euro füllen. Anschließend alle Waren entfernen. Einen neuen Artikel im Wert von 2 Euro in den Warenkorb legen.
        - **Erwartetes Ergebnis**: 5 Euro Versandkosten werden hinzugefügt.

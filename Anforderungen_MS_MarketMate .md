# Anforderungen

## **Die Applikation:**

Webshop mit folgenden Grundfunktionen:

- Registrierung und Login
- Produktsuche mit Sortierfunktion (z. B. nach Preis), Kategorisierung von Produkten
- Produkte zu Favoriten hinzufügen
- Produkte in den Warenkorb legen
- Bestellabschluss: Eingabe von Rechnungs- und Versandinformationen, Auswahl der Zahlungsmethode, Preisberechnung (Gesamtsumme)

---

## **Neue Funktionen**

### **1. Bewertungssystem für Produkte**

**Unklare Anforderung**:

- Nutzer sollen Produkte mit einem 5-Sterne-System bewerten und zusätzlich schriftliches Feedback hinterlassen können.

**Fragen**:

1. Was soll passieren, wenn eine Beschreibung aber keine Sternebewertung abgegeben wird?
2. Was passiert, wenn man eine Sternebewertungen abgibt aber keine schriftliche Bewertungen.
3. Was soll passieren, wenn ein Nutzer ein Produkt mehr als einmal bewerten möchte?
4. Was soll passieren, wenn ein Nutzer eine Bewertung löscht und das Produkt neu bewerten möchte?

**Detaillierte Anforderung**:

- Nutzer sollen nur die Möglichkeit haben, Bewertungen bei Produkten abzugeben, die sie gekauft haben. Das System soll zulassen, das Nutzer nur eine Sternebewertung ohne Beschreibung hinterlassen. Sollte keine Sternebewertung hinterlassen werden, wird eine Fehlermeldung angezeigt, dass das Rating Feld nicht leer sein darf.  Nutzer sollen die Möglichkeit haben ihre Bewertung zu löschen und eine neue Bewertung abzugeben.

---

### **2. Altersverifikation für alkoholische Produkte**

**Unklare Anforderung**:

- Alkoholische Produkte erfordern eine Altersverifikation. Beim Aufrufen der Kategorie soll ein Fenster erscheinen, in dem Nutzer ihr Alter angeben müssen (18+), bevor sie Zugriff erhalten.

**Fragen**:

1. Was soll passieren, wenn das Verifizierungsfenster weggeklickt wird, ohne ein Alter einzugeben
2. Was soll passieren, wenn man unter 18 ist?
3. Wann soll das System das Alter abfragen?
4. Was sollte der Nutzer sehen, wenn er nicht alkoholische Kategorien anklickt?
5. Wird das Alter immer abgefragt, wenn man die Kategorie Alkohol anklickt?

**Detaillierte Anforderung**:

- Nutzer sollten aufgefordert werden, ihr Geburtsdatum einzutippen, sobald die Kategorie “Alkohol” der Shopseite betreten wird. Wird ein Geburtstag eingetragen, dass auf Minderjährigkeit schließen lässt, soll das System bei der Kategorie Alkohol eine Underage Notice geben und keine Produkte in dieser Kategorie anzeigen. Andere Kategorien sollen normal angezeigt werden.

---

### **3. Änderungen bei den Versandkosten**

**Unklare Anforderung**:

- Versandkosten entfallen ab einem bestimmten Bestellwert. Darunter fallen Versandkosten an.

**Fragen**:

1. Ab welchem Wert entfallen die Versandkosten?
2. Was soll passieren, wenn der Wert erst überschritten und dann wieder unterschritten wird?
3. Was soll passieren, wenn der Benutzer den Warenkorb entleert und dann wieder füllt?

**Detaillierte Anforderung**:

- Das System soll automatisch die Versandkosten entfernen, wenn der Warenwert 20 Euro oder mehr beträgt. Die Versandkosten sollten wieder hinzugefügt werden, wenn der Warenwert weniger als 20 Euro beträgt. Wenn der Warenkorb entleert wird und mit neuen Waren gefüllt wird sollte er sich wie zuvor verhalten.
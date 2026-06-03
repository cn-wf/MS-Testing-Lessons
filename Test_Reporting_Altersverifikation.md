# Test Reporting Altersverifikation

Vorbereitung für die nachfolgenden Testfälle

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3 | Click on Create new account | You are directed to the signup page | OK | /auth |  |
| 4a | Fill in RandomName1 as Full Name |  |  |  |  |
| 4b | Fill in [random1@email.com](mailto:random@email.com) as Email |  |  |  |  |
| 4c | Fill in 123456789 as Password |  |  |  |  |
| 4d | Click on Sign Up | You are directed to the login page | OK |  |  |

## Scenario 1:  Überprüfung des Systemsverhaltens nach geschlossenem Altersverifikationsfenster

Der Nutzer sollte nach schließen des Altersverifikationsfensters als minderjährig gelten.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Click on Category “Alocohol” | No products are found. A underage notice appears. | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

![image.png](image.png)

![image.png](image%201.png)

## Scenario 2:  Überprüfung des Systemsverhaltens nach Alterseingabe von Heute - 17 Jahren

Der Nutzer sollte nach Eingabe eines Geburtsdatums von Heute - 17 Jahren als minderjährig gelten und Alkohol sollte nicht angezeigt werden.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 17 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 7 | Click on Category “Alocohol” | No products are found. A underage notice appears. | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

![image.png](image%202.png)

![image.png](image%203.png)

## Scenario 3:  Überprüfung des Systemsverhaltens nach Alterseingabe von Heute - 18 Jahren

Der Nutzer sollte nach Eingabe eines Geburtsdatums von Heute - 18 Jahren als volljährig gelten und Alkohol sollte angezeigt werden.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 18 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are of age message appears. | OK |  |  |
| 7 | Click on Category “Alocohol” | Alcoholic products can be seen | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

## Scenario 4:  Überprüfung des Systemsverhaltens nach Alterseingabe von Heute - 19 Jahren

Der Nutzer sollte nach Eingabe eines Geburtsdatums von Heute - 19 Jahren als volljährig gelten und Alkohol sollte angezeigt werden.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 19 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are of age message appears. | OK |  |  |
| 7 | Click on Category “Alocohol” | Alcoholic products can be seen | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

## Scenario 5: Überprüfen ob eine Alters Verifikation beim Betreten der Shopseite erfolgt oder bei der Navigation zur Kategorie Alkohol als volljährige Person

Als volljähriger Nutzer von Market Mate sollte ich eine Alterverifikation beim Betreten des Shopreiters durchführen und keine weitere beim öffnen der Kategorie Alkohol.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 18 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are of age message appears. | OK |  |  |
| 7 | Click on Category “Alocohol” | Alcoholic products can be seen. No Age Verification window opens. | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

## Scenario 6: Überprüfen ob eine Alters Verifikation beim Betreten der Shopseite erfolgt oder bei der Navigation zur Kategorie Alkohol als minderjährige Person

Als minderjähriger Nutzer von Market Mate sollte ich eine Alterverifikation beim Betreten des Shopreiters durchführen und keine weitere beim öffnen der Kategorie Alkohol.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 17 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 7 | Click on Category “Alocohol” | Alcoholic products cannot be seen. No Age Verification window opens. | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |

## Scenario 7: Überprüfung der Sichtbarkeit der Kategorien außer Alkohol für minderjährige Nutzer

Als minderjähriger Nutzer von Market Mate sollte ich alle Kategorien außer Alkohol sehen können.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Fill in todays date - 17 years |  |  |  |  |
| 6 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 7 | Click on Category “Fish” | Fish products can be seen.  | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
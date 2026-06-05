# Test Reporting Versandkosten

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

## Scenario 1:  Überprüfung der Versandkosten bei 20 Euro Warenwert

Der Nutzer sollte ab einem Warenwert von 20 Euro keine Versandkosten berechnet bekommen.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Add 10 “Gala Apples” to the Cart | 10 “Gala Apples” are added to the Cart | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
| 7 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 8 | Check if Shipment = 0 | Shipment cost = 0 | OK |  |  |

## Scenario 2:  Überprüfung der Versandkosten bei 22 Euro Warenwert

Der Nutzer sollte ab einem Warenwert von 22 Euro keine Versandkosten berechnet bekommen.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Add 11 “Gala Apples” to the Cart | 11 “Gala Apples” are added to the Cart | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
| 7 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 8 | Check if Shipment = 0 | Shipment cost = 0 | OK |  |  |

## Scenario 3:  Überprüfung der Versandkosten bei 18 Euro Warenwert

Der Nutzer sollte ab einem Warenwert von 22 Euro keine Versandkosten berechnet bekommen.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Add 9 “Gala Apples” to the Cart | 9 “Gala Apples” are added to the Cart | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
| 7 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 8 | Check if Shipment = 5 | Shipment cost = 5 | OK |  |  |

## Scenario 4:  Überprüfung der Versandkosten bei 18 Euro Warenwert nachdem 20 Euro erreicht wurden

Der Nutzer sollte bei 18 Euro Warenwert Versandkosten berechnet bekommen, auch wenn vorher 20 Euro Warenwert im Warenkorb vorhanden waren.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Add 10 “Gala Apples” to the Cart | 10 “Gala Apples” are added to the Cart | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
| 7 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 8 | Check if Shipment = 0 | Shipment cost = 0 | OK |  |  |
| 9 | Click on “-” button at apples amount | Amount of apples is reduced to 9 | OK |  |  |
| 10 | Check if Shipment = 5 | Shipment cost = 5 | NOK |  | [https://github.com/cn-wf/MS-Testing-Lessons/issues/1](https://github.com/cn-wf/MS-Testing-Lessons/issues/1) |

## Scenario 5:  Überprüfung der Versandkosten nachdem Waren hinzugefügt und wieder entfernt wurden

Der Nutzer sollte bei 2 Euro Warenwert Versandkosten berechnet bekommen, nachdem der Warenkorb vorher befüllt und wieder entleert wurde.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3a | Fill in random1@email.com as Email |  |  |  |  |
| 3b | Fill in 123456789 as Password |  |  |  |  |
| 3c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 4 | Click on Shop | You are directed to the shop page. Age Verification window opens. | OK | /store |  |
| 5 | Click on confirm | Age Verification window closes. You are underage message appears. | OK |  |  |
| 6 | Add 10 “Gala Apples” to the Cart | 10 “Gala Apples” are added to the Cart | OK | [https://grocerymate.masterschool.com/store#](https://grocerymate.masterschool.com/store#) |  |
| 7 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 8 | Check if Shipment = 0 Euros | Shipment cost = 0 Euros | OK |  |  |
| 9 | Click on “-” button at apples amount | Amount of apples is reduced to 9 | OK |  |  |
| 10 | Check if Shipment = 5 Euros | Shipment cost = 5 Euros | NOK |  | [https://github.com/cn-wf/MS-Testing-Lessons/issues/1](https://github.com/cn-wf/MS-Testing-Lessons/issues/1) |
| 11 | Click on ”-” nine times  | Cart should be empty | OK |  |  |
| 12 | Click on Shop | You are directed to the shop page.  | OK | [https://grocerymate.masterschool.com/store](https://grocerymate.masterschool.com/store) |  |
| 13 | Add 1 “Gala Apples” to the Cart | 1 “Gala Apples” is added to the Cart | OK |  |  |
| 14 | Click on Cart | You are directed to the cart page | OK | [https://grocerymate.masterschool.com/checkout](https://grocerymate.masterschool.com/checkout) |  |
| 15 | Check if Shipment = 5 Euros | Shipment cost = 5 Euros | OK |  |  |
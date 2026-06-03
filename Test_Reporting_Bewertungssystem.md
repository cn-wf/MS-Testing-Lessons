# Test Reporting

Vorbereitung für die nachfolgenden Testfälle

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on Login button | You are directed to the login page | OK | /auth |  |
| 3 | Click on Create new account | You are directed to the signup page | OK | /auth |  |
| 4a | Fill in RandomName as Full Name |  |  |  |  |
| 4b | Fill in [random@email.com](mailto:random@email.com) as Email |  |  |  |  |
| 4c | Fill in 123456789 as Password |  |  |  |  |
| 4d | Click on Sign Up | You are directed to the login page | OK |  |  |
| 5a | Fill in random@email.com as Email |  |  |  |  |
| 5b | Fill in 123456789 as Password |  |  |  |  |
| 5c | Click on Sign In | You are now logged in and are directed to the homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |

## Scenario 1:  Beschreibung ohne Rating abgeben

Als ein Nutzer von Market Mate sollte ich keine Beschreibung ohne Rating abgeben können.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 3a | Fill in 13.02.2000 in age verification |  |  |  |  |
| 3b | Click “confirm” on age verification window | verification disappears |  |  |  |
| 4 | Add 1 “Gala Apples” to Cart |  |  |  |  |
| 5 | Click on “Cart” | You are directed to cart page | OK | /checkout |  |
| 6a | Fill in RandomAddress |  |  |  |  |
| 6b | Fill in RandomCity |  |  |  |  |
| 6c | Fill in RandomPostalCode |  |  |  |  |
| 6d | Fill 123456789 as Card number |  |  |  |  |
| 6e | Fill in RandomName as Name of card |  |  |  |  |
| 6f | Fill 1234567 in Expiration |  |  |  |  |
| 6g | Fill 123 in Cvv |  |  |  |  |
| 6h | Click on Buy now | You “buy” the Product and are redirected to homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 7 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 8 | Click on “Gala Apples” | You are directed to review site for Gala Apples | OK | [https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998](https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998) |  |
| 9a | Click on “What is your view?” |  |  |  |  |
| 9b | Fill in Lorem Ipsum |  |  |  |  |
| 9c | Click on “Send” | You cannot send the Review and get a Error message  | OK |  |  |

![image.png](image.png)

## Scenario 2: Rating ohne Beschreibung abgeben

Als Nutzer von Market Mate sollte ich ein Rating ohne eine Beschreibung abgeben können.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 3a | Fill in 13.02.2000 in age verification |  |  |  |  |
| 3b | Click “confirm” on age verification window | verification disappears |  |  |  |
| 4 | Add 1 “Gala Apples” to Cart |  |  |  |  |
| 5 | Click on “Cart” | You are directed to cart page | OK | /checkout |  |
| 6a | Fill in RandomAddress |  |  |  |  |
| 6b | Fill in RandomCity |  |  |  |  |
| 6c | Fill in RandomPostalCode |  |  |  |  |
| 6d | Fill 123456789 as Card number |  |  |  |  |
| 6e | Fill in RandomName as Name of card |  |  |  |  |
| 6f | Fill 1234567 in Expiration |  |  |  |  |
| 6g | Fill 123 in Cvv |  |  |  |  |
| 6h | Click on Buy now | You “buy” the Product and are redirected to homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 7 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 8 | Click on “Gala Apples” | You are directed to review site for Gala Apples | OK | [https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998](https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998) |  |
| 9a | Click on the 4th star |  |  |  |  |
| 9b | Click on “Send” | You review window closes and your review get posted on top of the existing reviews | OK |  |  |

![image.png](image%201.png)

![image.png](image%202.png)

## Scenario 3: Versuch eine Zweite Bewertung abzugeben während die erste existiert

Als Nutzer von Market Mate sollte ich nicht die Möglichkeit haben, eine zweite Bewertung für ein bereits bewertetes Produkt zu geben.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 3a | Fill in 13.02.2000 in age verification |  |  |  |  |
| 3b | Click “confirm” on age verification window | verification disappears |  |  |  |
| 4 | Add 1 “Gala Apples” to Cart |  |  |  |  |
| 5 | Click on “Cart” | You are directed to cart page | OK | /checkout |  |
| 6a | Fill in RandomAddress |  |  |  |  |
| 6b | Fill in RandomCity |  |  |  |  |
| 6c | Fill in RandomPostalCode |  |  |  |  |
| 6d | Fill 123456789 as Card number |  |  |  |  |
| 6e | Fill in RandomName as Name of card |  |  |  |  |
| 6f | Fill 1234567 in Expiration |  |  |  |  |
| 6g | Fill 123 in Cvv |  |  |  |  |
| 6h | Click on Buy now | You “buy” the Product and are redirected to homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 7 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 8 | Click on “Gala Apples” | You are directed to review site for Gala Apples | OK | [https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998](https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998) |  |
| 9a | Click on the 4th star |  |  |  |  |
| 9b | Click on “Send” | You review window closes and your review get posted on top of the existing reviews | OK |  |  |
| 10 | Click on “Shop” | You are directed to the shop page | OK |  |  |
| 11 | Click on “Gala Apples” | You are directed to review site for Gala Apples, no new Review window is opened | OK |  |  |

![image.png](image%203.png)

## Scenario 4: Versuch eine Bewertung für ein bereits bewertetes Produkt abzugeben, bei dem die vorausgegangene Bewertung gelöscht wurde

Als Nutzer von Market Mate sollte ich die Möglichkeit haben, meine alte Bewertung zu löschen und eine neue Bewertung abzugeben.

| Step# | Action | Expected outcome | OK/NOT | URL | Link to issue |
| --- | --- | --- | --- | --- | --- |
| 1 | Go to Homepage of Market Mate | Homepage appears | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 2 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 3a | Fill in 13.02.2000 in age verification |  |  |  |  |
| 3b | Click “confirm” on age verification window | verification disappears |  |  |  |
| 4 | Add 1 “Gala Apples” to Cart |  |  |  |  |
| 5 | Click on “Cart” | You are directed to cart page | OK | /checkout |  |
| 6a | Fill in RandomAddress |  |  |  |  |
| 6b | Fill in RandomCity |  |  |  |  |
| 6c | Fill in RandomPostalCode |  |  |  |  |
| 6d | Fill 123456789 as Card number |  |  |  |  |
| 6e | Fill in RandomName as Name of card |  |  |  |  |
| 6f | Fill 1234567 in Expiration |  |  |  |  |
| 6g | Fill 123 in Cvv |  |  |  |  |
| 6h | Click on Buy now | You “buy” the Product and are redirected to homepage | OK | [https://grocerymate.masterschool.com/](https://grocerymate.masterschool.com/) |  |
| 7 | Click on “Shop” | You are directed to shop page | OK | /store |  |
| 8 | Click on “Gala Apples” | You are directed to review site for Gala Apples | OK | [https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998](https://grocerymate.masterschool.com/product/66b3a57b3fd5048eacb47998) |  |
| 9a | Click on the 4th star |  |  |  |  |
| 9b | Click on “Send” | You review window closes and your review get posted on top of the existing reviews | OK |  |  |
| 10 | Click on “Shop” | You are directed to the shop page | OK |  |  |
| 11 | Click on “Gala Apples” | You are directed to review site for Gala Apples, no new Review window is opened | OK |  |  |
| 12 | Click on “…” in your old review | You open a window with “Edit” and “Delete” options | OK |  |  |
| 13 | Click on “Delete” | A confirmation window is opened | OK |  |  |
| 14 | Click on “OK” in the confirmation window | Your old review is deleted and a new review window is opened | OK |  |  |
| 15a | Click on the 5th star |  |  |  |  |
| 15b | Click on “Send” | You review window closes and your review get posted on top of the existing reviews | OK |  |  |

![image.png](image%204.png)

![image.png](image%205.png)

![image.png](image%206.png)

![image.png](image%207.png)

![image.png](image%208.png)

![image.png](image%209.png)
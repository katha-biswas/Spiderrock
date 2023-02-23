SpiderRock FIX and Data Structures Challenge

FIX, Financial Information eXchange, is a human-readable Key/Value protocol used by securities
exchanges for Order Entry. The format is key=value with separators.
FIX has a set of rules for validation. Some examples:
- Tags cannot be repeated within a section
- Repeating groups start with a count field that must match the number of repeating groups
FIX has set of standard messages. Below are common order messages.
- 35=D, New Order Single messages can notify the exchange of a new order request.
- 35=8, Execution reports notify the client that an order has been accepted or filled.
Here is an example of a login message (35=A):
8=FIX.4.2|9=0020|35=A|49=INCA|56=BATS|34=000000001|50=0028|57=PROD|108=30|10=084|
For a more information please reference:
Financial Information eXchange - Wikipedia

Included is a text file with a set of fix messages using “|” as a separator.
In your language of choice, please write a sample program that reads these FIX messages and:
- Lists error notifications for messages that have the same field twice
- Lists the highest and lowest price of valid New Order Single messages by Account
Feel free to ask questions.

Questions for further discussion in interview:
How would you validate the field values?
Explain how FIX repeating groups work.
How would you validate the tags of repeating groups?

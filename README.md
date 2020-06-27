## How to generate pre-filled email links

1. Go to [TinyURL](tinyurl.com)
2. In the *Enter a long URL to make tiny* box enter the `mailto` line from below, filled out with email, cc, bcc, subject, and message
3. Click *Make TinyURL!*

## Email message template

This is a long line a characters that includes all of the information from the email message. A short tutorial is below.  You can find more doumentation from the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks#E-mail_links)

1. Start with `mailto:`
2. Next add the recipient's email address `mailto:person@example.com`
3. If you want to add another recipient just separate each address with a comma.  Don't put a space in there!
```
mailto:person@example.com,other-person@example.com
```
4. If you want to add a CC, BCC, a pre-filled subject or a pre-filled message, add a `?` after the addresses
5. To add a CC, add `cc=carbon-copy-person@example.com`.  You can add multiple separated by a comma.
6. To add even more (BCC, subject, message), we'll add a `?` and keep going.  Add a `?` after every step to separate the different parts. 
7. To add a BCC, add `bcc=secret-person@example.com`.  Again, you can add multiple separated by a comma.
8. To add a pre-filled subject, add `subject=This%20is%20%the%20%subject`.  Notice all the `%20`'s.  Those actually represent spaces because we can't have spaces in a link. You can [use this tool](https://meyerweb.com/eric/tools/dencoder/) to convert regular text into text for your subject and message.
9. To add a pre-filled message, convert your text with [the encoding tool](https://meyerweb.com/eric/tools/dencoder/) and add to to your string `body=fancy%20encoded%20message`

## Some Examples
mailto:test@example.org
mailto:test@example.org,other@example.org
mailto:test@example.org?cc=other@example.org&subject=This%20is%20the%20subject
mailto:test@example.org?body=This%20is%20the%20body
# Script: inbox-imap-shellnetrc

A script that shows if there are unread mails in your IMAP inbox.

For Gmail, you must allow [less secure apps](https://myaccount.google.com/security#connectedapps).

This script actually use imaps. curl can also handle IMAP or POP3. To do this, you only need to change the protocol in the command.

The login data is stored in a `.netrc`. This is more secure because the password is not visible in the process list.


## Dependencies

* `curl`


## Module

```
[module/inbox-imap-shellnetrc]
type = custom/script
exec = ~/polybar-scripts/inbox-imap-shellnetrc.sh
interval = 60
```
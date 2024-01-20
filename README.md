# Introduction

| Protocol | Port | Description |
| -------- | ---- | ----------- |
| SMTP     | 25   |             |
| SSL/TLS  | 465  |             |
| StartTLS | 587  |             |

```
MUA → MSA → MTA → internet → MTA → MDA → MUA
```

{% code overflow="wrap" %}
```
Outlook → Exchange → firewall → internet → SMTP-Server of the receiving side → mail-server
```
{% endcode %}

**SMTP Commands**

| Command   | Description                                  | RFC      |
| --------- | -------------------------------------------- | -------- |
| HELO      | Identifies the sending SMTP server           | RFC 5321 |
| EHLO      | Extended HELO, provides more information     | RFC 5321 |
| MAIL FROM | Specifies the sender’s email address         | RFC 5321 |
| RCPT TO   | Specifies the recipient’s email address      | RFC 5321 |
| DATA      | Initiates the message data transmission      | RFC 5321 |
| RSET      | Resets the session to initial state          | RFC 5321 |
| VRFY      | Requests verification of an email address    | RFC 5321 |
| EXPN      | Requests the expansion of a mailing list     | RFC 5321 |
| NOOP      | No operation, used for testing or keep-alive | RFC 5321 |
| QUIT      | Closes the SMTP session                      | RFC 5321 |
| AUTH      | Initiates authentication process             | RFC 4954 |
| STARTTLS  | Initiates a secure TLS session               | RFC 3207 |
| HELP      | Requests help information from the server    | RFC 5321 |

[**RFC 821**](https://datatracker.ietf.org/doc/html/rfc821.html) – Simple Mail Transfer Protocol

Protocol definition for SMTP. This document covers the model, operating procedure, and protocol details for SMTP.

[**RFC 1869**](https://datatracker.ietf.org/doc/html/rfc1869.html) – SMTP Service Extensions

Definition of the ESMTP extensions for SMTP. This describes a framework for extending SMTP with new commands, supporting dynamic discovery of the commands provided by the server, and defines a few additional commands.

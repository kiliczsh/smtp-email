# smtp-email

- Create base64 auth credentials:

`echo -n "\000myemail@mydomain.com\000myholypassword" | base64`

- Connect to smtp server:

`openssl s_client -starttls smtp -connect smtp.anymailserver.com:587 -crlf`

- Introduce or start new session

`helo myhostname`

- Authenticate your user

`auth plain base64authcredential`


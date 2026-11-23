# QUEUE Unique (signing-queue web page)

Web page for booking queues to meet Unique executives for document signing. Opened from the LINE official account through LIFF.

- Page: https://kanyanatchai59-eng.github.io/queue-unique/
- LINE (LIFF): https://liff.line.me/2012532401-ZUHWPMkd
- Backend: Google Apps Script web app, data in Google Sheets / Drive

This repository holds only the page (`index.html`). It contains no data, no employee records and no secrets: every request goes to the Apps Script backend, which checks the user's session before returning anything. Channel secrets and tokens live in Apps Script Script Properties.

`index.html` is generated from the Apps Script `Index.html` (same file, template values removed), so both links run the same screens.

| Link | Opens |
|---|---|
| `?view=book` | Book a queue |
| `?view=mine` | My queues |
| `?view=change` | Reschedule or cancel |
| `?view=history` | History |
| `?tour=1` | How to use |
| `?req=<request id>` | A request |

# Backlinks Monitoring

Verifies the presence of one or more urls on one or more web pages.

### Start Configuration :

- Urls (don't edit): `{{ $sys.data.keys()[0] }}`
- Custom Data (one by line) : `"https://[MY_SOURCE]" = "https://[URL_TO_CHECK]"`

You can add several sources and url to check by adding as many lines as you want in `Custom data`.

### Result :

- alert (True if link as not found on page)
- source (Url of the checked web page)
- link (link not found on the website)
- response_code (http code of the server)

Only links not found are stored in the result !
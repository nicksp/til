# Protecting cookies with HttpOnly

[HttpOnly cookies](https://www.owasp.org/index.php/HttpOnly) are those that can only be accessed by the server. Any attempt to access such cookie from client-side script is strictly forbidden. So that's a great way to protect cookies from most malicious JavaScript.

Cookies unavailable in JS code make huge classes of common XSS attacks much harder to pull off. Malicious code sneaked into the page is unable to steal user cookies with `document.cookie` command.

The good news is that it works in [all popular and modern browsers](http://www.browserscope.org/?category=security&v=top) (IE6+, Firefox 2.0+, Chrome 1.0+, Opera 9.5+, Safari 4.0+)

Here's what a cookie looks like with the `HttpOnly` flag set:

```
Set-Cookie: <name>=<value>[; <Max-Age>=<age>]
[; expires=<date>][; domain=<domain_name>]
[; path=<some_path>][; secure][; HttpOnly]
```

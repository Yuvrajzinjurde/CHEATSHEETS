`cookie-parser`

- cookie-parser middleware is used for parsing the cookies attached to the request object. when client sends a request tp your express server, it often includes cookies as part of the request heders. these cookies can contain data such as part of the request headers. these cookies can contain data such as session tokens, user preferences, authentication tokens, etc.

- The `cookie-parser` middleware parses these cookies and makes them available in a convenient format on the `req.cookies` object in subsequent route handler. This allows you to easily access and manipulate the cookies in your Express app.

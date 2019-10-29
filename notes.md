# Routing Notes

[ client ] == makes a request to an == [ api ] == sends a response back to the == [ client ]

what is the interface for a web api? ==>

- URI (Uniform Resource Identifier)
- URL (Universal Resource Locator),
- Endpoint (very related to a URI)
- HTTP === network protocol, a set rules for communication

REST(ish)

- everything is a `Resource`.
- single URI per resource. ex: `http://web23.com/channels`, `http://web23.com/users`.
- use HTTP METHODS to perform operations on resources.
- hypermedia (at this level we are fully REST).

| Non REST         | REST              |
| :--------------- | :---------------- |
| /listAllChannels | GET /channels     |
| /createChannel   | POST /channels    |
| /updateChannel   | PUT /channels     |
| /deleteChannel   | DELETE /channels  |
| /findChannel     | GET /channels/123 |

What is an Express Router? why is it useful?

An Express Router can have route/request handlers and middleware

## Query String

https://www.google.com/search?q=express+js&oq=express+js&aqs=chrome..69i57j0l4j69i65.1919j1j8&sourceid=chrome&ie=UTF-8

https://www.google.com/search
?
q = express+js
&
oq = express+js
&
ie = UTF-8

```js
req.query = {
  q: 'express+js',
  oq: 'express+js',
  ie: 'UTF-8',
};
```

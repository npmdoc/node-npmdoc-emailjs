# api documentation for  [emailjs (v1.0.8)](https://github.com/eleith/emailjs#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-emailjs.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-emailjs) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-emailjs.svg)](https://travis-ci.org/npmdoc/node-npmdoc-emailjs)
#### send text/html emails and attachments (files, streams and strings) from node.js to any smtp server

[![NPM](https://nodei.co/npm/emailjs.png?downloads=true)](https://www.npmjs.com/package/emailjs)

[![apidoc](https://npmdoc.github.io/node-npmdoc-emailjs/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-emailjs_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-emailjs/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-emailjs/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-emailjs/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "eleith"
    },
    "bugs": {
        "url": "https://github.com/eleith/emailjs/issues"
    },
    "contributors": [
        {
            "name": "izuzak"
        },
        {
            "name": "Hiverness"
        },
        {
            "name": "mscdex"
        },
        {
            "name": "jimmybergman"
        }
    ],
    "dependencies": {
        "addressparser": "^0.3.2",
        "bufferjs": "=1.1.0",
        "mimelib": "0.2.14",
        "moment": "= 2.11.2",
        "starttls": "1.0.1"
    },
    "description": "send text/html emails and attachments (files, streams and strings) from node.js to any smtp server",
    "devDependencies": {
        "chai": "= 1.1.0",
        "iconv": "2.1.6",
        "mailparser": "0.4.1",
        "mocha": "= 1.7.4",
        "simplesmtp": "0.3.32"
    },
    "directories": {},
    "dist": {
        "shasum": "d4240db7670dc78aff97352092d8460edc130f66",
        "tarball": "https://registry.npmjs.org/emailjs/-/emailjs-1.0.8.tgz"
    },
    "engine": [
        "node >= 0.10"
    ],
    "gitHead": "09a3b8e899f4f2e6287220bba5584f5ec4a0df30",
    "homepage": "https://github.com/eleith/emailjs#readme",
    "license": "MIT",
    "main": "email.js",
    "maintainers": [
        {
            "name": "eleith",
            "email": "work@eleith.com"
        }
    ],
    "name": "emailjs",
    "optionalDependencies": {
        "bufferjs": "=1.1.0"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/eleith/emailjs.git"
    },
    "scripts": {
        "test": "mocha -R spec -t 5000"
    },
    "version": "1.0.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module emailjs](#apidoc.module.emailjs)
1.  [function <span class="apidocSignatureSpan">emailjs.</span>SMTP.SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP)
1.  [function <span class="apidocSignatureSpan">emailjs.</span>message.Message (headers)](#apidoc.element.emailjs.message.Message)
1.  [function <span class="apidocSignatureSpan">emailjs.</span>server.Client (server)](#apidoc.element.emailjs.server.Client)
1.  object <span class="apidocSignatureSpan">emailjs.</span>SMTP
1.  object <span class="apidocSignatureSpan">emailjs.</span>SMTP.SMTP.prototype
1.  object <span class="apidocSignatureSpan">emailjs.</span>message
1.  object <span class="apidocSignatureSpan">emailjs.</span>message.Message.prototype
1.  object <span class="apidocSignatureSpan">emailjs.</span>response
1.  object <span class="apidocSignatureSpan">emailjs.</span>server
1.  object <span class="apidocSignatureSpan">emailjs.</span>server.Client.prototype

#### [module emailjs.SMTP](#apidoc.module.emailjs.SMTP)
1.  [function <span class="apidocSignatureSpan">emailjs.</span>SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP)
1.  object <span class="apidocSignatureSpan">emailjs.SMTP.</span>authentication
1.  object <span class="apidocSignatureSpan">emailjs.SMTP.</span>state

#### [module emailjs.SMTP.SMTP](#apidoc.module.emailjs.SMTP.SMTP)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.</span>SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP.SMTP)

#### [module emailjs.SMTP.SMTP.prototype](#apidoc.module.emailjs.SMTP.SMTP.prototype)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>addListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>authorized ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.authorized)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>close (force)](#apidoc.element.emailjs.SMTP.SMTP.prototype.close)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>command (cmd, callback, codes, failed)](#apidoc.element.emailjs.SMTP.SMTP.prototype.command)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>connect (callback, port, host, options)](#apidoc.element.emailjs.SMTP.SMTP.prototype.connect)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>data (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.data)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>data_end (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.data_end)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>debug (level)](#apidoc.element.emailjs.SMTP.SMTP.prototype.debug)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>ehlo (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>ehlo_or_helo_if_needed (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo_or_helo_if_needed)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>emit (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.emit)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>eventNames ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.eventNames)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>expn (address, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.expn)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>getMaxListeners ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.getMaxListeners)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>has_extn (opt)](#apidoc.element.emailjs.SMTP.SMTP.prototype.has_extn)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>helo (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.helo)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>help (callback, args)](#apidoc.element.emailjs.SMTP.SMTP.prototype.help)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>listenerCount (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.listenerCount)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>listeners (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>login (callback, user, password, options)](#apidoc.element.emailjs.SMTP.SMTP.prototype.login)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>mail (callback, from)](#apidoc.element.emailjs.SMTP.SMTP.prototype.mail)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>message (data)](#apidoc.element.emailjs.SMTP.SMTP.prototype.message)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>noop (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.noop)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>on (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.on)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>once (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.once)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>parse_smtp_features (data)](#apidoc.element.emailjs.SMTP.SMTP.prototype.parse_smtp_features)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>prependListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.prependOnceListener)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>quit (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.quit)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>rcpt (callback, to)](#apidoc.element.emailjs.SMTP.SMTP.prototype.rcpt)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>removeAllListeners (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>removeListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>rset (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.rset)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>send (str, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.send)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>setMaxListeners (n)](#apidoc.element.emailjs.SMTP.SMTP.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>starttls (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.starttls)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>state ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.state)
1.  [function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>verify (address, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.verify)
1.  undefined <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>domain

#### [module emailjs.message](#apidoc.module.emailjs.message)
1.  [function <span class="apidocSignatureSpan">emailjs.message.</span>Message (headers)](#apidoc.element.emailjs.message.Message)
1.  [function <span class="apidocSignatureSpan">emailjs.message.</span>create (headers)](#apidoc.element.emailjs.message.create)
1.  number <span class="apidocSignatureSpan">emailjs.message.</span>BUFFERSIZE

#### [module emailjs.message.Message](#apidoc.module.emailjs.message.Message)
1.  [function <span class="apidocSignatureSpan">emailjs.message.</span>Message (headers)](#apidoc.element.emailjs.message.Message.Message)

#### [module emailjs.message.Message.prototype](#apidoc.module.emailjs.message.Message.prototype)
1.  [function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>attach (options)](#apidoc.element.emailjs.message.Message.prototype.attach)
1.  [function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>attach_alternative (html, charset)](#apidoc.element.emailjs.message.Message.prototype.attach_alternative)
1.  [function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>read (callback)](#apidoc.element.emailjs.message.Message.prototype.read)
1.  [function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>stream ()](#apidoc.element.emailjs.message.Message.prototype.stream)
1.  [function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>valid (callback)](#apidoc.element.emailjs.message.Message.prototype.valid)

#### [module emailjs.response](#apidoc.module.emailjs.response)
1.  [function <span class="apidocSignatureSpan">emailjs.response.</span>monitor (stream, timeout, onerror)](#apidoc.element.emailjs.response.monitor)

#### [module emailjs.server](#apidoc.module.emailjs.server)
1.  [function <span class="apidocSignatureSpan">emailjs.server.</span>Client (server)](#apidoc.element.emailjs.server.Client)
1.  [function <span class="apidocSignatureSpan">emailjs.server.</span>connect (server)](#apidoc.element.emailjs.server.connect)

#### [module emailjs.server.Client](#apidoc.module.emailjs.server.Client)
1.  [function <span class="apidocSignatureSpan">emailjs.server.</span>Client (server)](#apidoc.element.emailjs.server.Client.Client)

#### [module emailjs.server.Client.prototype](#apidoc.module.emailjs.server.Client.prototype)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_connect (stack)](#apidoc.element.emailjs.server.Client.prototype._connect)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_containsInlinedHtml (attachment)](#apidoc.element.emailjs.server.Client.prototype._containsInlinedHtml)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_isAttachmentInlinedHtml (attachment)](#apidoc.element.emailjs.server.Client.prototype._isAttachmentInlinedHtml)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_poll ()](#apidoc.element.emailjs.server.Client.prototype._poll)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_senddata (stack)](#apidoc.element.emailjs.server.Client.prototype._senddata)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_senddone (err, stack)](#apidoc.element.emailjs.server.Client.prototype._senddone)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendmail (stack)](#apidoc.element.emailjs.server.Client.prototype._sendmail)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendmessage (stack)](#apidoc.element.emailjs.server.Client.prototype._sendmessage)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendrcpt (stack)](#apidoc.element.emailjs.server.Client.prototype._sendrcpt)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendsmtp (stack, next)](#apidoc.element.emailjs.server.Client.prototype._sendsmtp)
1.  [function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>send (msg, callback)](#apidoc.element.emailjs.server.Client.prototype.send)



# <a name="apidoc.module.emailjs"></a>[module emailjs](#apidoc.module.emailjs)

#### <a name="apidoc.element.emailjs.SMTP.SMTP"></a>[function <span class="apidocSignatureSpan">emailjs.</span>SMTP.SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP)
- description and source-code
```javascript
SMTP.SMTP = function (options) {
  events.EventEmitter.call(this);

  options = options || {};

  this.sock = null;
  this.timeout = options.timeout || TIMEOUT;
  this.features = null;
  this._state = SMTPState.NOTCONNECTED;
  this._secure = false;
  this.loggedin = (options.user && options.password) ? false : true;
  this.domain = options.domain || os.hostname();
  this.host = options.host || 'localhost';
  this.port = options.port || (options.ssl ? SMTP_SSL_PORT : options.tls ? SMTP_TLS_PORT : SMTP_PORT);
  this.ssl = options.ssl || false;
  this.tls = options.tls || false;
  this.monitor = null;
  this.authentication = options.authentication || [AUTH_METHODS.CRAM_MD5, AUTH_METHODS.LOGIN, AUTH_METHODS.PLAIN, AUTH_METHODS.XOAUTH2
];

  // keep these strings hidden when quicky debugging/logging
  this.user = function() {
    return options.user;
  };
  this.password = function() {
    return options.password;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.message.Message"></a>[function <span class="apidocSignatureSpan">emailjs.</span>message.Message (headers)](#apidoc.element.emailjs.message.Message)
- description and source-code
```javascript
message.Message = function (headers)
{
   this.attachments  = [];
   this.alternative  = null;
   var now = new Date();
   this.header       = {
      "message-id":"<" + now.getTime() + "." + (counter++) + "." + process.pid + "@" + os.hostname() +">",
      "date":moment().locale('en').format("ddd, DD MMM YYYY HH:mm:ss ZZ")
   };
   this.content      = "text/plain; charset=utf-8";

   for(var header in headers)
   {
      // allow user to override default content-type to override charset or send a single non-text message
      if(/^content-type$/i.test(header))
      {
         this.content = headers[header];
      }
      else if(header == 'text')
      {
         this.text = headers[header];
      }
      else if(header == "attachment" && typeof (headers[header]) == "object")
      {
         if(Array.isArray(headers[header])) {
            var that = this;

            for (var i = 0, l = headers[header].length; i < l; i++) {
              this.attach(headers[header][i]);
            }
         } else {
            this.attach(headers[header]);
         }
      }
      else if(header == 'subject')
      {
         this.header.subject = mimelib.encodeMimeWord(headers.subject, 'Q', 'utf-8');
      }
      else if(/^(cc|bcc|to|from)/i.test(header))
      {
         this.header[header.toLowerCase()] = person2address(headers[header]);
      }
      else
      {
         // allow any headers the user wants to set??
         // if(/cc|bcc|to|from|reply-to|sender|subject|date|message-id/i.test(header))
         this.header[header.toLowerCase()] = headers[header];
      }
   }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client"></a>[function <span class="apidocSignatureSpan">emailjs.</span>server.Client (server)](#apidoc.element.emailjs.server.Client)
- description and source-code
```javascript
server.Client = function (server)
{
   this.smtp         = new smtp.SMTP(server);
   //this.smtp.debug(1);

   this.queue        = [];
   this.timer        = null;
   this.sending      = false;
   this.ready        = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.SMTP"></a>[module emailjs.SMTP](#apidoc.module.emailjs.SMTP)

#### <a name="apidoc.element.emailjs.SMTP.SMTP"></a>[function <span class="apidocSignatureSpan">emailjs.</span>SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP)
- description and source-code
```javascript
SMTP = function (options) {
  events.EventEmitter.call(this);

  options = options || {};

  this.sock = null;
  this.timeout = options.timeout || TIMEOUT;
  this.features = null;
  this._state = SMTPState.NOTCONNECTED;
  this._secure = false;
  this.loggedin = (options.user && options.password) ? false : true;
  this.domain = options.domain || os.hostname();
  this.host = options.host || 'localhost';
  this.port = options.port || (options.ssl ? SMTP_SSL_PORT : options.tls ? SMTP_TLS_PORT : SMTP_PORT);
  this.ssl = options.ssl || false;
  this.tls = options.tls || false;
  this.monitor = null;
  this.authentication = options.authentication || [AUTH_METHODS.CRAM_MD5, AUTH_METHODS.LOGIN, AUTH_METHODS.PLAIN, AUTH_METHODS.XOAUTH2
];

  // keep these strings hidden when quicky debugging/logging
  this.user = function() {
    return options.user;
  };
  this.password = function() {
    return options.password;
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.SMTP.SMTP"></a>[module emailjs.SMTP.SMTP](#apidoc.module.emailjs.SMTP.SMTP)

#### <a name="apidoc.element.emailjs.SMTP.SMTP.SMTP"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.</span>SMTP (options)](#apidoc.element.emailjs.SMTP.SMTP.SMTP)
- description and source-code
```javascript
SMTP = function (options) {
  events.EventEmitter.call(this);

  options = options || {};

  this.sock = null;
  this.timeout = options.timeout || TIMEOUT;
  this.features = null;
  this._state = SMTPState.NOTCONNECTED;
  this._secure = false;
  this.loggedin = (options.user && options.password) ? false : true;
  this.domain = options.domain || os.hostname();
  this.host = options.host || 'localhost';
  this.port = options.port || (options.ssl ? SMTP_SSL_PORT : options.tls ? SMTP_TLS_PORT : SMTP_PORT);
  this.ssl = options.ssl || false;
  this.tls = options.tls || false;
  this.monitor = null;
  this.authentication = options.authentication || [AUTH_METHODS.CRAM_MD5, AUTH_METHODS.LOGIN, AUTH_METHODS.PLAIN, AUTH_METHODS.XOAUTH2
];

  // keep these strings hidden when quicky debugging/logging
  this.user = function() {
    return options.user;
  };
  this.password = function() {
    return options.password;
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.SMTP.SMTP.prototype"></a>[module emailjs.SMTP.SMTP.prototype](#apidoc.module.emailjs.SMTP.SMTP.prototype)

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.addListener"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>addListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.addListener)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.authorized"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>authorized ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.authorized)
- description and source-code
```javascript
authorized = function () {
  return this.loggedin;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.close"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>close (force)](#apidoc.element.emailjs.SMTP.SMTP.prototype.close)
- description and source-code
```javascript
close = function (force) {
  if (this.sock) {
    if (force) {
      log("smtp connection destroyed!");
      this.sock.destroy();
    } else {
      log("smtp connection closed.");
      this.sock.end();
    }
  }

  if (this.monitor) {
    this.monitor.stop();
    this.monitor = null;
  }

  this._state = SMTPState.NOTCONNECTED;
  this._secure = false;
  this.sock = null;
  this.features = null;
  this.loggedin = !(this.user() && this.password());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.command"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>command (cmd, callback, codes, failed)](#apidoc.element.emailjs.SMTP.SMTP.prototype.command)
- description and source-code
```javascript
command = function (cmd, callback, codes, failed) {
  codes = Array.isArray(codes) ? codes : typeof(codes) == 'number' ? [codes] : [250];

  var response = function(err, msg) {
    if (err) {
      caller(callback, err);
    } else {
      if (codes.indexOf(Number(msg.code)) != -1) {
        caller(callback, err, msg.data, msg.message);
      } else {
        var errorMessage = "bad response on command '" + cmd.split(' ')[0] + "'";
        if (msg.message) {
          errorMessage += ': ' + msg.message;
        }
        caller(callback, SMTPError(errorMessage, SMTPError.BADRESPONSE, null, msg.data));
      }
    }
  };

  this.send(cmd + CRLF, response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.connect"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>connect (callback, port, host, options)](#apidoc.element.emailjs.SMTP.SMTP.prototype.connect)
- description and source-code
```javascript
connect = function (callback, port, host, options) {
  options = options || {};

  var self = this;

  self.host = host || self.host;
  self.port = port || self.port;
  self.ssl = options.ssl || self.ssl;

  if (self._state != SMTPState.NOTCONNECTED) {
    self.quit(function() {
      self.connect(callback, port, host, options);
    });
    return;
  }

  var connected = function(err) {
    if (!err) {
      log("connected: " + self.host + ":" + self.port);

      if (self.ssl && !self.tls) {
        // if key/ca/cert was passed in, check if connection is authorized
        if (typeof(self.ssl) != 'boolean' && !self.sock.authorized) {
          self.close(true);
          caller(callback, SMTPError('could not establish an ssl connection', SMTPError.CONNECTIONAUTH, err));
        } else self._secure = true;
      }
    } else {
      self.close(true);
      caller(callback, SMTPError("could not connect", SMTPError.COULDNOTCONNECT, err));
    }
  };

  var response = function(err, msg) {
    if (err) {
      if (self._state === SMTPState.NOTCONNECTED && !self.sock) {
        return;
      }
      self.close(true);
      caller(callback, err);
    } else if (msg.code == '220') {
      log(msg.data);

      // might happen first, so no need to wait on connected()
      self._state = SMTPState.CONNECTED;
      caller(callback, null, msg.data);
    } else {
      log("response (data): " + msg.data);
      self.quit(function() {
        caller(callback, SMTPError("bad response on connection", SMTPError.BADRESPONSE, err, msg.data));
      });
    }
  };

  self._state = SMTPState.CONNECTING;
  log("connecting: " + self.host + ":" + self.port);

  if (self.ssl) {
    self.sock = tls.connect(self.port, self.host, self.ssl, connected);
  } else {
    self.sock = new net.Socket();
    self.sock.connect(self.port, self.host, connected);
  }

  self.monitor = SMTPResponse.monitor(self.sock, self.timeout, function() {
    self.close(true);
  });
  self.sock.once('response', response);
  self.sock.once('error', response); // the socket could reset or throw, so let's handle it and let the user know
}
```
- example usage
```shell
...
 - auth access to an SMTP Server
 - if your service (ex: gmail) uses two-step authentication, use an application specific password

## EXAMPLE USAGE - text only emails

'''javascript
var email 	= require("./path/to/emailjs/email");
var server 	= email.server.connect({
   user:    "username",
   password:"password",
   host:    "smtp.your-email.com",
   ssl:     true
});

// send the message and get a callback with an error or details of the message that was sent
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.data"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>data (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.data)
- description and source-code
```javascript
data = function (callback) {
  this.command("data", callback, [354]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.data_end"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>data_end (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.data_end)
- description and source-code
```javascript
data_end = function (callback) {
  this.command(CRLF + ".", callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.debug"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>debug (level)](#apidoc.element.emailjs.SMTP.SMTP.prototype.debug)
- description and source-code
```javascript
debug = function (level) {
  DEBUG = level;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>ehlo (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo)
- description and source-code
```javascript
ehlo = function (callback, domain) {
  var self = this,

    response = function(err, data) {
      if (err) {
        caller(callback, err);
      } else {
        self.parse_smtp_features(data);

        if (self.tls && !self._secure) {
          self.starttls(function() {
            self.ehlo(callback, domain);
          });
        } else {
          caller(callback, err, data);
        }
      }
    };

  this.features = {};
  this.command("ehlo " + (domain || this.domain), response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo_or_helo_if_needed"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>ehlo_or_helo_if_needed (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.ehlo_or_helo_if_needed)
- description and source-code
```javascript
ehlo_or_helo_if_needed = function (callback, domain) {
  // Call self.ehlo() and/or self.helo() if needed.
  // If there has been no previous EHLO or HELO command self session, self
  //  method tries ESMTP EHLO first.
  var self = this;

  if (!this.features) {
    var response = function(err, data) {
      caller(callback, err, data);
    };

    var attempt = function(err, data) {
      if (err) self.helo(response, domain);
      else caller(callback, err, data);
    };

    self.ehlo(attempt, domain);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.emit"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>emit (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.emit)
- description and source-code
```javascript
function emit(type) {
  var er, handler, len, args, i, events, domain;
  var needDomainExit = false;
  var doError = (type === 'error');

  events = this._events;
  if (events)
    doError = (doError && events.error == null);
  else if (!doError)
    return false;

  domain = this.domain;

  // If there is no 'error' event listener then throw.
  if (doError) {
    er = arguments[1];
    if (domain) {
      if (!er)
        er = new Error('Uncaught, unspecified "error" event');
      er.domainEmitter = this;
      er.domain = domain;
      er.domainThrown = false;
      domain.emit('error', er);
    } else if (er instanceof Error) {
      throw er; // Unhandled 'error' event
    } else {
      // At least give some kind of context to the user
      var err = new Error('Uncaught, unspecified "error" event. (' + er + ')');
      err.context = er;
      throw err;
    }
    return false;
  }

  handler = events[type];

  if (!handler)
    return false;

  if (domain && this !== process) {
    domain.enter();
    needDomainExit = true;
  }

  var isFn = typeof handler === 'function';
  len = arguments.length;
  switch (len) {
    // fast cases
    case 1:
      emitNone(handler, isFn, this);
      break;
    case 2:
      emitOne(handler, isFn, this, arguments[1]);
      break;
    case 3:
      emitTwo(handler, isFn, this, arguments[1], arguments[2]);
      break;
    case 4:
      emitThree(handler, isFn, this, arguments[1], arguments[2], arguments[3]);
      break;
    // slower
    default:
      args = new Array(len - 1);
      for (i = 1; i < len; i++)
        args[i - 1] = arguments[i];
      emitMany(handler, isFn, this, args);
  }

  if (needDomainExit)
    domain.exit();

  return true;
}
```
- example usage
```shell
...
    var line = buffer.replace("\r", '');

    if(!line.trim().split(/\n/).pop().match(/^(\d{3})\s/))
        return;

    var match = line ? line.match(/(\d+)\s?(.*)/) : null;

    stream.emit('response', null, match ? {code:match[1], message:match[2], data:line} : {code:-1, data:line});
    buffer = '';
  }
},

error = function(err)
{
  stream.emit('response', SMTPError('connection encountered an error', SMTPError.ERROR, err));
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.eventNames"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>eventNames ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.eventNames)
- description and source-code
```javascript
function eventNames() {
  return this._eventsCount > 0 ? Reflect.ownKeys(this._events) : [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.expn"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>expn (address, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.expn)
- description and source-code
```javascript
expn = function (address, callback) {
  // SMTP 'expn' command -- expands a mailing list.
  this.command("expn " + address, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.getMaxListeners"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>getMaxListeners ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.getMaxListeners)
- description and source-code
```javascript
function getMaxListeners() {
  return $getMaxListeners(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.has_extn"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>has_extn (opt)](#apidoc.element.emailjs.SMTP.SMTP.prototype.has_extn)
- description and source-code
```javascript
has_extn = function (opt) {
  return this.features[opt.toLowerCase()] === undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.helo"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>helo (callback, domain)](#apidoc.element.emailjs.SMTP.SMTP.prototype.helo)
- description and source-code
```javascript
helo = function (callback, domain) {
<span class="apidocCodeCommentSpan">  /*
   * SMTP 'helo' command.
   * Hostname to send for self command defaults to the FQDN of the local
   * host.
   */
</span>
  var self = this,

    response = function(err, data) {
      if (err) {
        caller(callback, err);
      } else {
        self.parse_smtp_features(data);
        caller(callback, err, data);
      }
    };

  this.command("helo " + (domain || this.domain), response);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.help"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>help (callback, args)](#apidoc.element.emailjs.SMTP.SMTP.prototype.help)
- description and source-code
```javascript
help = function (callback, args) {
  // SMTP 'help' command, returns text from the server
  this.command(args ? "help " + args : "help", callback, [211, 214]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.listenerCount"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>listenerCount (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.listenerCount)
- description and source-code
```javascript
function listenerCount(type) {
  const events = this._events;

  if (events) {
    const evlistener = events[type];

    if (typeof evlistener === 'function') {
      return 1;
    } else if (evlistener) {
      return evlistener.length;
    }
  }

  return 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.listeners"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>listeners (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.listeners)
- description and source-code
```javascript
function listeners(type) {
  var evlistener;
  var ret;
  var events = this._events;

  if (!events)
    ret = [];
  else {
    evlistener = events[type];
    if (!evlistener)
      ret = [];
    else if (typeof evlistener === 'function')
      ret = [evlistener];
    else
      ret = arrayClone(evlistener, evlistener.length);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.login"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>login (callback, user, password, options)](#apidoc.element.emailjs.SMTP.SMTP.prototype.login)
- description and source-code
```javascript
login = function (callback, user, password, options) {
  var self = this,

    login = {
      user: user ? function() {
        return user;
      } : self.user,
      password: password ? function() {
        return password;
      } : self.password,
      method: options && options.method ? options.method.toUpperCase() : ''
    },

    domain = options && options.domain ? options.domain : this.domain,

    initiate = function(err, data) {
      if (err) {
        caller(callback, err);
        return;
      }

<span class="apidocCodeCommentSpan">      /*
       * Log in on an SMTP server that requires authentication.
       *
       * The arguments are:
       *     - user:     The user name to authenticate with.
       *     - password: The password for the authentication.
       *
       * If there has been no previous EHLO or HELO command self session, self
       * method tries ESMTP EHLO first.
       *
       * This method will return normally if the authentication was successful.
       */
</span>
      var method = null,

        encode_cram_md5 = function(challenge) {
          challenge = (new Buffer(challenge, "base64")).toString("ascii");

          var hmac = crypto.createHmac('md5', login.password());
          hmac.update(challenge);

          return (new Buffer(login.user() + " " + hmac.digest('hex')).toString("base64"));
        },

        encode_plain = function() {
          return (new Buffer("\u0000" + login.user() + "\u0000" + login.password())).toString("base64");
        },

        encode_xoauth2 = function() {
          // console.log("user=" + login.user() + "\1auth=Bearer " + login.password()+"\1\1");
          // see: https://developers.google.com/gmail/xoauth2_protocol
          return (new Buffer("user=" + login.user() + "\u0001auth=Bearer " + login.password() + "\u0001\u0001")).toString("base64
");
        };

      // List of authentication methods we support: from preferred to
      // less preferred methods.
      if (!method) {
        var preferred = self.authentication;

        for (var i = 0; i < preferred.length; i++) {
          if ((self.features.auth || "").indexOf(preferred[i]) != -1) {
            method = preferred[i];
            break;
          }
        }
      }

      // handle bad responses from command differently
      var failed = function(err, data) {
        self.loggedin = false;
        self.close(); // if auth is bad, close the connection, it won't get better by itself
        caller(callback, SMTPError('authorization.failed', SMTPError.AUTHFAILED, err, data));
      };

      var response = function(err, data) {
        if (err) {
          failed(err, data);
        } else {
          self.loggedin = true;
          caller(callback, err, data);
        }
      };

      var attempt = function(err, data, msg) {
        if (err) {
          failed(err, data);
        } else {
          if (method == AUTH_METHODS.CRAM_MD5) {
            self.command(encode_cram_md5(msg), response, [235, 503]);
          } else if (method == AUTH_METHODS.LOGIN) {
            self.command((new Buffer(login.password())).toString("base64"), response, [235, 503]);
          }
        }
      };

      var attempt_user = function(err, data, msg) {
        if (err) {
          failed(err, data);
        } else {
          if (method == AUTH_METHODS.LOGIN) {
            self.command((new Buffer(login.user())).toString("base64"), attempt, [334]);
          }
        }
      };

      if (method == AUTH_METHODS.CRAM_MD5) self.command("AUTH " + AUTH_METHODS.CRAM_MD5, attempt, [334]);

      else if (method == AUTH_METHODS.LOGIN) self.command("AUTH " + AUTH_METHODS.LOGIN, attempt_user, [334]);

      else if (method == AUTH_METHODS.PLAIN) self.command("AUTH " + AUTH_METHODS.PLAIN + " " + encode_plain(login.user(), login.
password()), response, [235, 503]);

      else if (method == AUTH_METHODS.XOAUTH2) self.command("AUTH " + AUTH_METHODS.XOAUTH2 + " " + encode_xoauth2(login.user(),
login.password()), response, [235, 503]);

      else if (!method) caller(callback, SMTPError('no form of authorization supported', SMTPError.AUTHNOTSU ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.mail"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>mail (callback, from)](#apidoc.element.emailjs.SMTP.SMTP.prototype.mail)
- description and source-code
```javascript
mail = function (callback, from) {
  this.command("mail FROM:" + from, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.message"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>message (data)](#apidoc.element.emailjs.SMTP.SMTP.prototype.message)
- description and source-code
```javascript
message = function (data) {
  log(data);
  this.sock.write(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.noop"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>noop (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.noop)
- description and source-code
```javascript
noop = function (callback) {
  this.send("noop", callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.on"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>on (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.on)
- description and source-code
```javascript
function addListener(type, listener) {
  return _addListener(this, type, listener, false);
}
```
- example usage
```shell
...
    stream.removeListener('close', close);
    stream.removeListener('error', error);

    if(err && typeof(onerror) == "function")
      onerror(err);
  };

  //stream.on('readable', watch);
  stream.on('data', watch);
  stream.on('end', end);
  stream.on('close', close);
  stream.on('error', error);
  stream.setTimeout(timeout, timedout);
};
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.once"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>once (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.once)
- description and source-code
```javascript
function once(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.on(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.parse_smtp_features"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>parse_smtp_features (data)](#apidoc.element.emailjs.SMTP.SMTP.prototype.parse_smtp_features)
- description and source-code
```javascript
parse_smtp_features = function (data) {
  var self = this;

  //  According to RFC1869 some (badly written)
  //  MTA's will disconnect on an ehlo. Toss an exception if
  //  that happens -ddm

  data.split("\n").forEach(function(ext) {
    var parse = ext.match(/^(?:\d+[\-=]?)\s*?([^\s]+)(?:\s+(.*)\s*?)?$/);

    // To be able to communicate with as many SMTP servers as possible,
    // we have to take the old-style auth advertisement into account,
    // because:
    // 1) Else our SMTP feature parser gets confused.
    // 2) There are some servers that only advertise the auth methods we
    // support using the old style.

    if (parse) {
      // RFC 1869 requires a space between ehlo keyword and parameters.
      // It's actually stricter, in that only spaces are allowed between
      // parameters, but were not going to check for that here.  Note
      // that the space isn't present if there are no parameters.
      self.features[parse[1].toLowerCase()] = parse[2] || true;
    }
  });

  return;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>prependListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.prependListener)
- description and source-code
```javascript
function prependListener(type, listener) {
  return _addListener(this, type, listener, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.prependOnceListener"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>prependOnceListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.prependOnceListener)
- description and source-code
```javascript
function prependOnceListener(type, listener) {
  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');
  this.prependListener(type, _onceWrap(this, type, listener));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.quit"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>quit (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.quit)
- description and source-code
```javascript
quit = function (callback) {
  var self = this,
    response = function(err, data) {
      caller(callback, err, data);
      self.close();
    };

  this.command("quit", response, [221, 250]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.rcpt"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>rcpt (callback, to)](#apidoc.element.emailjs.SMTP.SMTP.prototype.rcpt)
- description and source-code
```javascript
rcpt = function (callback, to) {
  this.command("RCPT TO:" + to, callback, [250, 251]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>removeAllListeners (type)](#apidoc.element.emailjs.SMTP.SMTP.prototype.removeAllListeners)
- description and source-code
```javascript
function removeAllListeners(type) {
  var listeners, events;

  events = this._events;
  if (!events)
    return this;

  // not listening for removeListener, no need to emit
  if (!events.removeListener) {
    if (arguments.length === 0) {
      this._events = new EventHandlers();
      this._eventsCount = 0;
    } else if (events[type]) {
      if (--this._eventsCount === 0)
        this._events = new EventHandlers();
      else
        delete events[type];
    }
    return this;
  }

  // emit removeListener for all listeners on all events
  if (arguments.length === 0) {
    var keys = Object.keys(events);
    for (var i = 0, key; i < keys.length; ++i) {
      key = keys[i];
      if (key === 'removeListener') continue;
      this.removeAllListeners(key);
    }
    this.removeAllListeners('removeListener');
    this._events = new EventHandlers();
    this._eventsCount = 0;
    return this;
  }

  listeners = events[type];

  if (typeof listeners === 'function') {
    this.removeListener(type, listeners);
  } else if (listeners) {
    // LIFO order
    do {
      this.removeListener(type, listeners[listeners.length - 1]);
    } while (listeners[0]);
  }

  return this;
}
```
- example usage
```shell
...

  end = function(err)
  {
stream.emit('response', SMTPError('connection has ended', SMTPError.CONNECTIONENDED, err));
  };

  this.stop = function(err) {
stream.removeAllListeners('response');
//stream.removeListener('readable', watch);
stream.removeListener('data', watch);
stream.removeListener('end', end);
stream.removeListener('close', close);
stream.removeListener('error', error);

if(err && typeof(onerror) == "function")
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>removeListener (type, listener)](#apidoc.element.emailjs.SMTP.SMTP.prototype.removeListener)
- description and source-code
```javascript
function removeListener(type, listener) {
  var list, events, position, i, originalListener;

  if (typeof listener !== 'function')
    throw new TypeError('"listener" argument must be a function');

  events = this._events;
  if (!events)
    return this;

  list = events[type];
  if (!list)
    return this;

  if (list === listener || list.listener === listener) {
    if (--this._eventsCount === 0)
      this._events = new EventHandlers();
    else {
      delete events[type];
      if (events.removeListener)
        this.emit('removeListener', type, list.listener || listener);
    }
  } else if (typeof list !== 'function') {
    position = -1;

    for (i = list.length; i-- > 0;) {
      if (list[i] === listener || list[i].listener === listener) {
        originalListener = list[i].listener;
        position = i;
        break;
      }
    }

    if (position < 0)
      return this;

    if (list.length === 1) {
      list[0] = undefined;
      if (--this._eventsCount === 0) {
        this._events = new EventHandlers();
        return this;
      } else {
        delete events[type];
      }
    } else {
      spliceOne(list, position);
    }

    if (events.removeListener)
      this.emit('removeListener', type, originalListener || listener);
  }

  return this;
}
```
- example usage
```shell
...
  end = function(err)
  {
stream.emit('response', SMTPError('connection has ended', SMTPError.CONNECTIONENDED, err));
  };

  this.stop = function(err) {
stream.removeAllListeners('response');
//stream.removeListener('readable', watch);
stream.removeListener('data', watch);
stream.removeListener('end', end);
stream.removeListener('close', close);
stream.removeListener('error', error);

if(err && typeof(onerror) == "function")
  onerror(err);
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.rset"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>rset (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.rset)
- description and source-code
```javascript
rset = function (callback) {
  this.command("rset", callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.send"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>send (str, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.send)
- description and source-code
```javascript
send = function (str, callback) {
  var self = this;

  if (self.sock && self._state == SMTPState.CONNECTED) {
    log(str);

    var response = function(err, msg) {
      if (err) {
        caller(callback, err);
      } else {
        log(msg.data);
        caller(callback, null, msg);
      }
    };

    self.sock.once('response', response);
    self.sock.write(str);
  } else {
    self.close(true);
    caller(callback, SMTPError('no connection has been established', SMTPError.NOCONNECTION));
  }
}
```
- example usage
```shell
...
   user:    "username",
   password:"password",
   host:    "smtp.your-email.com",
   ssl:     true
});

// send the message and get a callback with an error or details of the message that was sent
server.send({
   text:    "i hope this works",
   from:    "you <username@your-email.com>",
   to:      "someone <someone@your-email.com>, another <another@your-email.com>",
   cc:      "else <else@your-email.com>",
   subject: "testing emailjs"
}, function(err, message) { console.log(err || message); });
'''
...
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>setMaxListeners (n)](#apidoc.element.emailjs.SMTP.SMTP.prototype.setMaxListeners)
- description and source-code
```javascript
function setMaxListeners(n) {
  if (typeof n !== 'number' || n < 0 || isNaN(n))
    throw new TypeError('"n" argument must be a positive number');
  this._maxListeners = n;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.starttls"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>starttls (callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.starttls)
- description and source-code
```javascript
starttls = function (callback) {
  var self = this,

    response = function(err, msg) {
      if (err) {
        err.message += " while establishing a starttls session";
        caller(callback, err);
      } else {
        // support new API
        if (tls.TLSSocket) {
          var secured_socket = new tls.TLSSocket(self.sock, {
            secureContext: tls.createSecureContext ? tls.createSecureContext(self.tls) : crypto.createCredentials(self.tls),
            isServer: false // older versions of node (0.12), do not default to false properly...
          });

          secured_socket.on('error', function(err) {
            self.close(true);
            caller(callback, err);
          });

          self._secure = true;
          self.sock = secured_socket;

          SMTPResponse.monitor(self.sock, self.timeout, function() {
            self.close(true);
          });
          caller(callback, msg.data);
        } else {
          var secured_socket = null;
          var secured = function() {
            self._secure = true;
            self.sock = secured_socket;

            var error = function(err) {
              self.close(true);
              caller(callback, err);
            };

            SMTPResponse.monitor(self.sock, self.timeout, function() {
              self.close(true);
            });
            caller(callback, msg.data);
          };

          //secured_socket = starttls.secure(self.sock, self.tls, secured);
          var starttls = require('starttls');
          secured_socket = starttls({
            socket: self.sock,
            host: self.host,
            port: self.port,
            pair: tls.createSecurePair(
              tls.createSecureContext ? tls.createSecureContext(self.tls) : crypto.createCredentials(self.tls),
              false)
          }, secured).cleartext;

          secured_socket.on('error', function(err) {
            self.close(true);
            caller(callback, err);
          });
        }
      }
    };

  this.command("starttls", response, [220]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.state"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>state ()](#apidoc.element.emailjs.SMTP.SMTP.prototype.state)
- description and source-code
```javascript
state = function () {
  return this._state;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.SMTP.SMTP.prototype.verify"></a>[function <span class="apidocSignatureSpan">emailjs.SMTP.SMTP.prototype.</span>verify (address, callback)](#apidoc.element.emailjs.SMTP.SMTP.prototype.verify)
- description and source-code
```javascript
verify = function (address, callback) {
  // SMTP 'verify' command -- checks for address validity."""
  this.command("vrfy " + address, callback, [250, 251, 252]);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.message"></a>[module emailjs.message](#apidoc.module.emailjs.message)

#### <a name="apidoc.element.emailjs.message.Message"></a>[function <span class="apidocSignatureSpan">emailjs.message.</span>Message (headers)](#apidoc.element.emailjs.message.Message)
- description and source-code
```javascript
Message = function (headers)
{
   this.attachments  = [];
   this.alternative  = null;
   var now = new Date();
   this.header       = {
      "message-id":"<" + now.getTime() + "." + (counter++) + "." + process.pid + "@" + os.hostname() +">",
      "date":moment().locale('en').format("ddd, DD MMM YYYY HH:mm:ss ZZ")
   };
   this.content      = "text/plain; charset=utf-8";

   for(var header in headers)
   {
      // allow user to override default content-type to override charset or send a single non-text message
      if(/^content-type$/i.test(header))
      {
         this.content = headers[header];
      }
      else if(header == 'text')
      {
         this.text = headers[header];
      }
      else if(header == "attachment" && typeof (headers[header]) == "object")
      {
         if(Array.isArray(headers[header])) {
            var that = this;

            for (var i = 0, l = headers[header].length; i < l; i++) {
              this.attach(headers[header][i]);
            }
         } else {
            this.attach(headers[header]);
         }
      }
      else if(header == 'subject')
      {
         this.header.subject = mimelib.encodeMimeWord(headers.subject, 'Q', 'utf-8');
      }
      else if(/^(cc|bcc|to|from)/i.test(header))
      {
         this.header[header.toLowerCase()] = person2address(headers[header]);
      }
      else
      {
         // allow any headers the user wants to set??
         // if(/cc|bcc|to|from|reply-to|sender|subject|date|message-id/i.test(header))
         this.header[header.toLowerCase()] = headers[header];
      }
   }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.message.create"></a>[function <span class="apidocSignatureSpan">emailjs.message.</span>create (headers)](#apidoc.element.emailjs.message.create)
- description and source-code
```javascript
create = function (headers)
{
   return new Message(headers);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.message.Message"></a>[module emailjs.message.Message](#apidoc.module.emailjs.message.Message)

#### <a name="apidoc.element.emailjs.message.Message.Message"></a>[function <span class="apidocSignatureSpan">emailjs.message.</span>Message (headers)](#apidoc.element.emailjs.message.Message.Message)
- description and source-code
```javascript
Message = function (headers)
{
   this.attachments  = [];
   this.alternative  = null;
   var now = new Date();
   this.header       = {
      "message-id":"<" + now.getTime() + "." + (counter++) + "." + process.pid + "@" + os.hostname() +">",
      "date":moment().locale('en').format("ddd, DD MMM YYYY HH:mm:ss ZZ")
   };
   this.content      = "text/plain; charset=utf-8";

   for(var header in headers)
   {
      // allow user to override default content-type to override charset or send a single non-text message
      if(/^content-type$/i.test(header))
      {
         this.content = headers[header];
      }
      else if(header == 'text')
      {
         this.text = headers[header];
      }
      else if(header == "attachment" && typeof (headers[header]) == "object")
      {
         if(Array.isArray(headers[header])) {
            var that = this;

            for (var i = 0, l = headers[header].length; i < l; i++) {
              this.attach(headers[header][i]);
            }
         } else {
            this.attach(headers[header]);
         }
      }
      else if(header == 'subject')
      {
         this.header.subject = mimelib.encodeMimeWord(headers.subject, 'Q', 'utf-8');
      }
      else if(/^(cc|bcc|to|from)/i.test(header))
      {
         this.header[header.toLowerCase()] = person2address(headers[header]);
      }
      else
      {
         // allow any headers the user wants to set??
         // if(/cc|bcc|to|from|reply-to|sender|subject|date|message-id/i.test(header))
         this.header[header.toLowerCase()] = headers[header];
      }
   }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.message.Message.prototype"></a>[module emailjs.message.Message.prototype](#apidoc.module.emailjs.message.Message.prototype)

#### <a name="apidoc.element.emailjs.message.Message.prototype.attach"></a>[function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>attach (options)](#apidoc.element.emailjs.message.Message.prototype.attach)
- description and source-code
```javascript
attach = function (options)
{
<span class="apidocCodeCommentSpan">   /*
      legacy support, will remove eventually...
      arguments -> (path, type, name, headers)
   */
</span>   if (arguments.length > 1)
     options = {path:options, type:arguments[1], name:arguments[2]};

   // sender can specify an attachment as an alternative
   if(options.alternative)
   {
      this.alternative           = options;
      this.alternative.charset   = options.charset || "utf-8";
      this.alternative.type      = options.type || "text/html";
      this.alternative.inline    = true;
   }
   else
      this.attachments.push(options);

   return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.message.Message.prototype.attach_alternative"></a>[function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>attach_alternative (html, charset)](#apidoc.element.emailjs.message.Message.prototype.attach_alternative)
- description and source-code
```javascript
attach_alternative = function (html, charset)
{
   this.alternative =
   {
      data:    html,
      charset: charset || "utf-8",
      type:    "text/html",
      inline:  true
   };

   return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.message.Message.prototype.read"></a>[function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>read (callback)](#apidoc.element.emailjs.message.Message.prototype.read)
- description and source-code
```javascript
read = function (callback)
{
   var buffer = "";

   var capture = function(data)
   {
      buffer += data;
   };

   var output = function(err)
   {
      callback(err, buffer);
   };

   var str = this.stream();

   str.on('data', capture);
   str.on('end', output);
   str.on('error', output);
}
```
- example usage
```shell
...
  {
    stream.end();
    stream.emit('response', SMTPError('timedout while connecting to smtp server', SMTPError.TIMEDOUT, err));
  },

  watch = function(data)
  {
    //var data = stream.read();
    if (data !== null) {
var decoded = data.toString();
var emit		= false;
var code		= 0;

buffer += decoded;
notify();
...
```

#### <a name="apidoc.element.emailjs.message.Message.prototype.stream"></a>[function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>stream ()](#apidoc.element.emailjs.message.Message.prototype.stream)
- description and source-code
```javascript
stream = function ()
{
   return new MessageStream(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.message.Message.prototype.valid"></a>[function <span class="apidocSignatureSpan">emailjs.message.Message.prototype.</span>valid (callback)](#apidoc.element.emailjs.message.Message.prototype.valid)
- description and source-code
```javascript
valid = function (callback)
{
   var self = this;

   if(!self.header.from)
   {
      callback(false, "message does not have a valid sender");
   }
   if(!(self.header.to || self.header.cc || self.header.bcc))
   {
      callback(false, "message does not have a valid recipient");
   }
   else if(self.attachments.length === 0)
   {
      callback(true);
   }
   else
   {
      var check  = [];
      var failed = [];

      self.attachments.forEach(function(attachment, index)
      {
         if(attachment.path)
         {
            // migrating path->fs for existsSync)
            if(!(fs.existsSync || path.existsSync)(attachment.path))
               failed.push(attachment.path + " does not exist");
         }
         else if(attachment.stream)
         {
            if(!attachment.stream.readable)
               failed.push("attachment stream is not readable");
         }
         else if(!attachment.data)
         {
            failed.push("attachment has no data associated with it");
         }
      });

      callback(failed.length === 0, failed.join(", "));
   }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.response"></a>[module emailjs.response](#apidoc.module.emailjs.response)

#### <a name="apidoc.element.emailjs.response.monitor"></a>[function <span class="apidocSignatureSpan">emailjs.response.</span>monitor (stream, timeout, onerror)](#apidoc.element.emailjs.response.monitor)
- description and source-code
```javascript
monitor = function (stream, timeout, onerror)
{
  return new SMTPResponse(stream, timeout, onerror);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.server"></a>[module emailjs.server](#apidoc.module.emailjs.server)

#### <a name="apidoc.element.emailjs.server.Client"></a>[function <span class="apidocSignatureSpan">emailjs.server.</span>Client (server)](#apidoc.element.emailjs.server.Client)
- description and source-code
```javascript
Client = function (server)
{
   this.smtp         = new smtp.SMTP(server);
   //this.smtp.debug(1);

   this.queue        = [];
   this.timer        = null;
   this.sending      = false;
   this.ready        = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.connect"></a>[function <span class="apidocSignatureSpan">emailjs.server.</span>connect (server)](#apidoc.element.emailjs.server.connect)
- description and source-code
```javascript
connect = function (server)
{
   return new Client(server);
}
```
- example usage
```shell
...
 - auth access to an SMTP Server
 - if your service (ex: gmail) uses two-step authentication, use an application specific password

## EXAMPLE USAGE - text only emails

'''javascript
var email 	= require("./path/to/emailjs/email");
var server 	= email.server.connect({
   user:    "username",
   password:"password",
   host:    "smtp.your-email.com",
   ssl:     true
});

// send the message and get a callback with an error or details of the message that was sent
...
```



# <a name="apidoc.module.emailjs.server.Client"></a>[module emailjs.server.Client](#apidoc.module.emailjs.server.Client)

#### <a name="apidoc.element.emailjs.server.Client.Client"></a>[function <span class="apidocSignatureSpan">emailjs.server.</span>Client (server)](#apidoc.element.emailjs.server.Client.Client)
- description and source-code
```javascript
Client = function (server)
{
   this.smtp         = new smtp.SMTP(server);
   //this.smtp.debug(1);

   this.queue        = [];
   this.timer        = null;
   this.sending      = false;
   this.ready        = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.emailjs.server.Client.prototype"></a>[module emailjs.server.Client.prototype](#apidoc.module.emailjs.server.Client.prototype)

#### <a name="apidoc.element.emailjs.server.Client.prototype._connect"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_connect (stack)](#apidoc.element.emailjs.server.Client.prototype._connect)
- description and source-code
```javascript
_connect = function (stack)
{
   var self = this,

   connect = function(err)
   {
      if(!err)
      {
         var begin = function(err)
         {
            if(!err)
            {
               self.ready = true;
               self._poll();
            }
            else {
               stack.callback(err, stack.message);

               // clear out the queue so all callbacks can be called with the same error message
               self.queue.shift();
               self._poll();
            }
         };

         if(!self.smtp.authorized())
            self.smtp.login(begin);

         else
            self.smtp.ehlo_or_helo_if_needed(begin);
      }
      else {
         stack.callback(err, stack.message);

         // clear out the queue so all callbacks can be called with the same error message
         self.queue.shift();
         self._poll();
      }
   };

   self.ready = false;
   self.smtp.connect(connect);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._containsInlinedHtml"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_containsInlinedHtml (attachment)](#apidoc.element.emailjs.server.Client.prototype._containsInlinedHtml)
- description and source-code
```javascript
_containsInlinedHtml = function (attachment) {
	   if (Array.isArray(attachment)) {
		   return attachment.some((function(ctx) {
			   return function(att) {
				   return ctx._isAttachmentInlinedHtml(att);
			   };
		   })(this));
	   } else {
		   return this._isAttachmentInlinedHtml(attachment);
	   }
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._isAttachmentInlinedHtml"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_isAttachmentInlinedHtml (attachment)](#apidoc.element.emailjs.server.Client.prototype._isAttachmentInlinedHtml)
- description and source-code
```javascript
_isAttachmentInlinedHtml = function (attachment) {
	   return attachment &&
		  (attachment.data || attachment.path) &&
		   attachment.alternative === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._poll"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_poll ()](#apidoc.element.emailjs.server.Client.prototype._poll)
- description and source-code
```javascript
_poll = function ()
{
   var self = this;

   clearTimeout(self.timer);

   if(self.queue.length)
   {
      if(self.smtp.state() == smtp.state.NOTCONNECTED)
         self._connect(self.queue[0]);

      else if(self.smtp.state() == smtp.state.CONNECTED && !self.sending && self.ready)
         self._sendmail(self.queue.shift());
   }
   // wait around 1 seconds in case something does come in, otherwise close out SMTP connection if still open
   else if(self.smtp.state() == smtp.state.CONNECTED)
      self.timer = setTimeout(function() { self.smtp.quit(); }, 1000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._senddata"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_senddata (stack)](#apidoc.element.emailjs.server.Client.prototype._senddata)
- description and source-code
```javascript
_senddata = function (stack)
{
   var self = this;
   self.smtp.data(self._sendsmtp(stack, self._sendmessage));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._senddone"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_senddone (err, stack)](#apidoc.element.emailjs.server.Client.prototype._senddone)
- description and source-code
```javascript
_senddone = function (err, stack)
{
   var self = this;
   self.sending = false;
   stack.callback(err, stack.message);
   self._poll();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._sendmail"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendmail (stack)](#apidoc.element.emailjs.server.Client.prototype._sendmail)
- description and source-code
```javascript
_sendmail = function (stack)
{
   var self = this;
   var from = stack.returnPath || stack.from;
   self.sending = true;
   self.smtp.mail(self._sendsmtp(stack, self._sendrcpt), '<' + from + '>');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._sendmessage"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendmessage (stack)](#apidoc.element.emailjs.server.Client.prototype._sendmessage)
- description and source-code
```javascript
_sendmessage = function (stack)
{
   var self = this, stream = stack.message.stream();

   stream.on('data', function(data) { self.smtp.message(data); });
   stream.on('end', function() { self.smtp.data_end(self._sendsmtp(stack, function() { self._senddone(null, stack) })); });

   // there is no way to cancel a message while in the DATA portion, so we have to close the socket to prevent
   // a bad email from going out
   stream.on('error', function(err) { self.smtp.close(); self._senddone(err, stack); });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._sendrcpt"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendrcpt (stack)](#apidoc.element.emailjs.server.Client.prototype._sendrcpt)
- description and source-code
```javascript
_sendrcpt = function (stack)
{
   var self = this, to = stack.to.shift().address;
   self.smtp.rcpt(self._sendsmtp(stack, stack.to.length ? self._sendrcpt : self._senddata), '<'+ to +'>');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype._sendsmtp"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>_sendsmtp (stack, next)](#apidoc.element.emailjs.server.Client.prototype._sendsmtp)
- description and source-code
```javascript
_sendsmtp = function (stack, next)
{
   var self   = this;
   var check= function(err)
   {
      if(!err && next)
      {
         next.apply(self, [stack]);
      }
      else
      {
         // if we snag on SMTP commands, call done, passing the error
         // but first reset SMTP state so queue can continue polling
         self.smtp.rset(function() { self._senddone(err, stack); });
      }
   };

   return check;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.emailjs.server.Client.prototype.send"></a>[function <span class="apidocSignatureSpan">emailjs.server.Client.prototype.</span>send (msg, callback)](#apidoc.element.emailjs.server.Client.prototype.send)
- description and source-code
```javascript
send = function (msg, callback)
{
   var self = this;

   if(!(msg instanceof message.Message)
       && msg.from
       && (msg.to || msg.cc || msg.bcc)
       && (msg.text || this._containsInlinedHtml(msg.attachment)))
      msg = message.create(msg);

   if(msg instanceof message.Message)
   {
      msg.valid(function(valid, why)
      {
         if(valid)
         {
            var stack =
            {
               message:    msg,
               to:         addressparser(msg.header.to),
               from:       addressparser(msg.header.from)[0].address,
               callback:   callback || function() {}
            };

            if(msg.header.cc)
               stack.to = stack.to.concat(addressparser(msg.header.cc));

            if(msg.header.bcc)
               stack.to = stack.to.concat(addressparser(msg.header.bcc));

            if(msg.header['return-path'] && addressparser(msg.header['return-path']).length)
              stack.returnPath = addressparser(msg.header['return-path'])[0].address;

            self.queue.push(stack);
            self._poll();
         }
         else
            callback(new Error(why), msg);
      });
   }
   else
      callback(new Error("message is not a valid Message instance"), msg);
}
```
- example usage
```shell
...
   user:    "username",
   password:"password",
   host:    "smtp.your-email.com",
   ssl:     true
});

// send the message and get a callback with an error or details of the message that was sent
server.send({
   text:    "i hope this works",
   from:    "you <username@your-email.com>",
   to:      "someone <someone@your-email.com>, another <another@your-email.com>",
   cc:      "else <else@your-email.com>",
   subject: "testing emailjs"
}, function(err, message) { console.log(err || message); });
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)

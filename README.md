# api documentation for  [ftpd (v0.2.15)](https://github.com/sstur/nodeftpd#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ftpd.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ftpd) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ftpd.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ftpd)
#### Node FTP Server

[![NPM](https://nodei.co/npm/ftpd.png?downloads=true)](https://www.npmjs.com/package/ftpd)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ftpd/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ftpd_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ftpd/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ftpd/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ftpd/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "sstur"
    },
    "bugs": {
        "url": "https://github.com/sstur/nodeftpd/issues"
    },
    "contributors": [
        {
            "name": "Alex Drummond",
            "url": "https://github.com/addrummond"
        },
        {
            "name": "Eric Fong",
            "url": "https://github.com/ericfong"
        },
        {
            "name": "headconnect",
            "url": "https://github.com/headconnect"
        },
        {
            "name": "Andrew Johnston",
            "url": "https://github.com/billywhizz"
        },
        {
            "name": "José F. Romaniello",
            "url": "https://github.com/jfromaniello"
        },
        {
            "name": "Simon Sturmer",
            "url": "https://github.com/sstur"
        },
        {
            "name": "Alan Szlosek",
            "url": "https://github.com/alanszlosek"
        },
        {
            "name": "asylumfunk",
            "url": "https://github.com/asylumfunk"
        }
    ],
    "dependencies": {
        "dateformat": "1.0.7-1.2.3"
    },
    "description": "Node FTP Server",
    "devDependencies": {
        "async": "~0.1.15",
        "istanbul": "~0.2.4",
        "jsftp": "git://github.com/sergi/jsftp.git#master",
        "mocha": "~1.17.1",
        "should": "~3.1.2"
    },
    "directories": {},
    "dist": {
        "shasum": "877ead07ce6b5bd8b4c6e9ea270510924bbd099d",
        "tarball": "https://registry.npmjs.org/ftpd/-/ftpd-0.2.15.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "c2a54b331c76deae611ddf28077c69a4e42b7374",
    "homepage": "https://github.com/sstur/nodeftpd#readme",
    "keywords": [
        "ftp",
        "ftp-server",
        "ftpd"
    ],
    "license": "BSD-2-Clause",
    "main": "./lib/ftpd.js",
    "maintainers": [
        {
            "name": "sstur",
            "email": "sstur@me.com"
        }
    ],
    "name": "ftpd",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/sstur/nodeftpd.git"
    },
    "scripts": {
        "test": "istanbul test _mocha"
    },
    "version": "0.2.15"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ftpd](#apidoc.module.ftpd)
1.  [function <span class="apidocSignatureSpan">ftpd.</span>FtpServer (host, options)](#apidoc.element.ftpd.FtpServer)
1.  object <span class="apidocSignatureSpan">ftpd.</span>FtpServer.prototype
1.  object <span class="apidocSignatureSpan">ftpd.</span>glob
1.  object <span class="apidocSignatureSpan">ftpd.</span>starttls

#### [module ftpd.FtpServer](#apidoc.module.ftpd.FtpServer)
1.  [function <span class="apidocSignatureSpan">ftpd.</span>FtpServer (host, options)](#apidoc.element.ftpd.FtpServer.FtpServer)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.</span>super_ ()](#apidoc.element.ftpd.FtpServer.super_)

#### [module ftpd.FtpServer.prototype](#apidoc.module.ftpd.FtpServer.prototype)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_logIf (level, message, conn, isError)](#apidoc.element.ftpd.FtpServer.prototype._logIf)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_onConnection (socket)](#apidoc.element.ftpd.FtpServer.prototype._onConnection)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_traceIf (level, message, conn)](#apidoc.element.ftpd.FtpServer.prototype._traceIf)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>close ()](#apidoc.element.ftpd.FtpServer.prototype.close)
1.  [function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>listen ()](#apidoc.element.ftpd.FtpServer.prototype.listen)

#### [module ftpd.glob](#apidoc.module.ftpd.glob)
1.  [function <span class="apidocSignatureSpan">ftpd.</span>glob (path, fsm, callback, noWildcards)](#apidoc.element.ftpd.glob.glob)
1.  [function <span class="apidocSignatureSpan">ftpd.glob.</span>matchPattern (pattern, string)](#apidoc.element.ftpd.glob.matchPattern)
1.  [function <span class="apidocSignatureSpan">ftpd.glob.</span>setMaxStatsAtOnce (n)](#apidoc.element.ftpd.glob.setMaxStatsAtOnce)

#### [module ftpd.starttls](#apidoc.module.ftpd.starttls)
1.  [function <span class="apidocSignatureSpan">ftpd.starttls.</span>starttlsClient (socket, options, callback)](#apidoc.element.ftpd.starttls.starttlsClient)
1.  [function <span class="apidocSignatureSpan">ftpd.starttls.</span>starttlsServer (socket, options, callback)](#apidoc.element.ftpd.starttls.starttlsServer)
1.  string <span class="apidocSignatureSpan">ftpd.starttls.</span>RECOMMENDED_CIPHERS



# <a name="apidoc.module.ftpd"></a>[module ftpd](#apidoc.module.ftpd)

#### <a name="apidoc.element.ftpd.FtpServer"></a>[function <span class="apidocSignatureSpan">ftpd.</span>FtpServer (host, options)](#apidoc.element.ftpd.FtpServer)
- description and source-code
```javascript
function FtpServer(host, options) {
  var self = this;
  events.EventEmitter.call(self);

  self.host = host;

  self.options = options;

  if (!self.options.maxStatsAtOnce)
    self.options.maxStatsAtOnce = 5;

  if (!options.getInitialCwd)
    throw new Error("'getInitialCwd' option of FtpServer must be set");
  if (!options.getRoot)
    throw new Error("'getRoot' option of FtpServer must be set");
  self.getInitialCwd = options.getInitialCwd;
  self.getRoot = options.getRoot;

  self.getUsernameFromUid = options.getUsernameFromUid || function(uid, c) {
    c(null, "ftp");
  };
  self.getGroupFromGid = options.getGroupFromGid || function(gid, c) {
    c(null, "ftp");
  };
  self.debugging = options.logLevel || 0;
  self.useWriteFile = options.useWriteFile;
  self.useReadFile = options.useReadFile;
  self.uploadMaxSlurpSize = options.uploadMaxSlurpSize || 0;

  self.server = net.createServer();
  self.server.on('connection', function(socket) {
    self._onConnection(socket);
  });
  self.server.on('error', function(err) {
    self.emit('error', err);
  });
  self.server.on('close', function() {
    self.emit('close');
  });
}
```
- example usage
```shell
...
console.log();
console.log('*** To run as FTPS server,                 ***');
console.log('***  set "KEY_FILE", "CERT_FILE"           ***');
console.log('***  and (optionally) "CA_FILES" env vars. ***');
console.log();
}

server = new ftpd.FtpServer(options.host, {
getInitialCwd: function () {
  return '/';
},
getRoot: function () {
  return process.cwd();
},
pasvPortRangeStart: 1025,
...
```



# <a name="apidoc.module.ftpd.FtpServer"></a>[module ftpd.FtpServer](#apidoc.module.ftpd.FtpServer)

#### <a name="apidoc.element.ftpd.FtpServer.FtpServer"></a>[function <span class="apidocSignatureSpan">ftpd.</span>FtpServer (host, options)](#apidoc.element.ftpd.FtpServer.FtpServer)
- description and source-code
```javascript
function FtpServer(host, options) {
  var self = this;
  events.EventEmitter.call(self);

  self.host = host;

  self.options = options;

  if (!self.options.maxStatsAtOnce)
    self.options.maxStatsAtOnce = 5;

  if (!options.getInitialCwd)
    throw new Error("'getInitialCwd' option of FtpServer must be set");
  if (!options.getRoot)
    throw new Error("'getRoot' option of FtpServer must be set");
  self.getInitialCwd = options.getInitialCwd;
  self.getRoot = options.getRoot;

  self.getUsernameFromUid = options.getUsernameFromUid || function(uid, c) {
    c(null, "ftp");
  };
  self.getGroupFromGid = options.getGroupFromGid || function(gid, c) {
    c(null, "ftp");
  };
  self.debugging = options.logLevel || 0;
  self.useWriteFile = options.useWriteFile;
  self.useReadFile = options.useReadFile;
  self.uploadMaxSlurpSize = options.uploadMaxSlurpSize || 0;

  self.server = net.createServer();
  self.server.on('connection', function(socket) {
    self._onConnection(socket);
  });
  self.server.on('error', function(err) {
    self.emit('error', err);
  });
  self.server.on('close', function() {
    self.emit('close');
  });
}
```
- example usage
```shell
...
console.log();
console.log('*** To run as FTPS server,                 ***');
console.log('***  set "KEY_FILE", "CERT_FILE"           ***');
console.log('***  and (optionally) "CA_FILES" env vars. ***');
console.log();
}

server = new ftpd.FtpServer(options.host, {
getInitialCwd: function () {
  return '/';
},
getRoot: function () {
  return process.cwd();
},
pasvPortRangeStart: 1025,
...
```

#### <a name="apidoc.element.ftpd.FtpServer.super_"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.</span>super_ ()](#apidoc.element.ftpd.FtpServer.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ftpd.FtpServer.prototype"></a>[module ftpd.FtpServer.prototype](#apidoc.module.ftpd.FtpServer.prototype)

#### <a name="apidoc.element.ftpd.FtpServer.prototype._logIf"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_logIf (level, message, conn, isError)](#apidoc.element.ftpd.FtpServer.prototype._logIf)
- description and source-code
```javascript
_logIf = function (level, message, conn, isError) {
  if (this.debugging >= level) {
    if (conn)
      console.log((conn & conn.socket ? conn.socket.remoteAddress + ": " : "") + message);
    else
      console.log(message);

    if (isError) {
      console.trace("Trace follows");
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.FtpServer.prototype._onConnection"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_onConnection (socket)](#apidoc.element.ftpd.FtpServer.prototype._onConnection)
- description and source-code
```javascript
_onConnection = function (socket) {
  var conn = new FtpConnection({
    server: this,
    socket: socket,
    pasv: null, // passive listener server
    dataPort: 20,
    dataHost: null,
    dataListener: null, // for incoming passive connections
    dataSocket: null, // the actual data socket
    // True if the client has sent a PORT/PASV command, and
    // we haven't experienced a problem with the configuration
    // it specified. (This can therefore be true even if there
    // is not currently an open data connection.)
    dataConfigured: false,
    mode: "ascii",
    filefrom: "",
    username: null,
    filename: "",
    fs: null,
    cwd: null,
    root: null,
    hasQuit: false,

    // State for handling TLS upgrades.
    secure: false,
    pbszReceived: false
  });

  this.emit("client:connected", conn); // pass client info so they can listen for client-specific events

  socket.setTimeout(0);
  socket.setNoDelay();

  this._logIf(1, "Connection");
  conn.respond("220 FTP server (nodeftpd) ready");

  socket.on('data', function(buf) {
    conn._onData(buf);
  });
  socket.on('end', function() {
    conn._onEnd();
  });
  socket.on('close', function() {
    conn._onClose();
  });
  socket.on('error', function(err) {
    conn._onError(err);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.FtpServer.prototype._traceIf"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>_traceIf (level, message, conn)](#apidoc.element.ftpd.FtpServer.prototype._traceIf)
- description and source-code
```javascript
_traceIf = function (level, message, conn) {
  return this._logIf(level, message, conn, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.FtpServer.prototype.close"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>close ()](#apidoc.element.ftpd.FtpServer.prototype.close)
- description and source-code
```javascript
close = function () {
  return this.server[fname].apply(this.server, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.FtpServer.prototype.listen"></a>[function <span class="apidocSignatureSpan">ftpd.FtpServer.prototype.</span>listen ()](#apidoc.element.ftpd.FtpServer.prototype.listen)
- description and source-code
```javascript
listen = function () {
  return this.server[fname].apply(this.server, arguments);
}
```
- example usage
```shell
...
    } else {
      failure();
    }
  });
});

server.debugging = 4;
server.listen(options.port);
console.log('Listening on port ' + options.port);
...
```



# <a name="apidoc.module.ftpd.glob"></a>[module ftpd.glob](#apidoc.module.ftpd.glob)

#### <a name="apidoc.element.ftpd.glob.glob"></a>[function <span class="apidocSignatureSpan">ftpd.</span>glob (path, fsm, callback, noWildcards)](#apidoc.element.ftpd.glob.glob)
- description and source-code
```javascript
function glob(path, fsm, callback, noWildcards) {
  var s = path.indexOf('*');
  var q = path.indexOf('?');
  var w;
  for (w = 0; !noWildcards && w < path.length && path.charAt(w) != '*' && path.charAt(w) != '?'; ++w);

  if (w == path.length) { // There are no wildcards.
    fsm.readdir(path, function(err, contents) {
      if (err) {
        if (err.errno == constants.ENOTDIR) {
          statList(fsm, [path], function(err, list) {
            if (err)
              return callback(err);
            if (list.length != 1)
              throw new Error("Internal error in glob.js");
            callback(null, list);
          });
        }
        else if (err.errno == constants.ENOENT) {
          callback(null, []);
        }
        else {
          callback(err);
        }
      }
      else {
        statList(fsm, contents.map(function(p) {
          return PathModule.join(path, p);
        }), function(err, list) {
          if (err)
            callback(err);
          else
            callback(null, list);
        });
      }
    });

    return;
  }
  else {
    // Check that there is no '/' after the first wildcard.

    var i;
    for (i = w; i < path.length; ++i) {
      if (path.charAt(i) == '/')
        return callback(null, []);
    }

    var base = "", pattern;
    for (i = w; i >= 0; --i) {
      if (path.charAt(i) == '/') {
        base = path.substr(0, i + 1)
        break;
      }
    }
    pattern = path.substr(i == 0 ? 0 : i + 1);

    // Remove any leading/trailing slashes which might still
    // be present if the path contains multiple slashes.
    for (i = 0; i < pattern.length && pattern.charAt(i) == '/'; ++i);
    if (i > 0)
      pattern = pattern.substr(i);
    for (i = base.length - 1; i > 0 && base.charAt(i) == '/'; --i);
    if (i != base.length - 1)
      base = base.substr(0, i + 1);

    // We now have the base path in 'base' (possibly the empty string)
    // and the wildcard filename pattern in 'pattern'.

    readTheDir(false);
    function readTheDir(listingSingleDir) {
      fsm.readdir(base, function(err, contents) {
        if (err) {
          if (err.errno == constants.ENOTDIR || err.errno == constants.ENOENT) {
            callback(null, []);
          }
          else {
            callback(err);
          }
        }
        else {
          var matches;
          if (!listingSingleDir)
            matches = contents.filter(function(n) {
              return matchPattern(pattern, n);
            });
          else
            matches = contents;

          // Special case. If we have exactly one match, and it's a directory, then list
          // the contents of that directory. (There's no reason why anyone should want
          // to identify mutliple directories using wildcards and then list all of their
          // contents over FTP!)
          if (!listingSingleDir && matches.length == 1) {
            var dir = PathModule.join(base, matches[0]);
            fsm.stat(dir, function(err, st) {
              if (err)
                return callback(err);

              if (!st.isDirectory()) {
                doTheNormalThing();
              }
              else {
                base = dir;
                readTheDir(/*listingSingleDir=*/true);
              }
            });
          }
          else {
            doTheNormalThing();
          }

          function doTheNormalThing() {
            statList(fsm, matches.map(function(p) {
              return PathModule.join(base, p);
            }), function(err, list) {
              if (err)
                callback(err);
              else
                callback(null, list);
            });
          }
        }
      });
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.glob.matchPattern"></a>[function <span class="apidocSignatureSpan">ftpd.glob.</span>matchPattern (pattern, string)](#apidoc.element.ftpd.glob.matchPattern)
- description and source-code
```javascript
function matchPattern(pattern, string) {
  var pi = 0, si = 0;
  for (; si < string.length && pi < pattern.length; ++si) {
    var c = string.charAt(si);
    var pc = pattern.charAt(pi);

    if (pc == '*') {
      if (pi + 1 == pattern.length) {
        ;
      }
      else if (pattern.charAt(pi + 1) == '*') {
        --si;
        ++pi;
      }
      else if (pattern.charAt(pi + 1) == '?') {
        ++pi;
      }
      else if (si < string.length - 1 && pattern.charAt(pi + 1) == string.charAt(si)) {
        pi += 2;
      }
    }
    else if (pc == '?') {
      ++pi;
    }
    else if (pc == c) {
      ++pi;
    }
    else {
      return false;
    }
  }

  return (pi == pattern.length || (pi == pattern.length - 1 && pattern.charAt(pi) == '*')) &&
      si == string.length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.glob.setMaxStatsAtOnce"></a>[function <span class="apidocSignatureSpan">ftpd.glob.</span>setMaxStatsAtOnce (n)](#apidoc.element.ftpd.glob.setMaxStatsAtOnce)
- description and source-code
```javascript
function setMaxStatsAtOnce(n) {
  CONC = n;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.ftpd.starttls"></a>[module ftpd.starttls](#apidoc.module.ftpd.starttls)

#### <a name="apidoc.element.ftpd.starttls.starttlsClient"></a>[function <span class="apidocSignatureSpan">ftpd.starttls.</span>starttlsClient (socket, options, callback)](#apidoc.element.ftpd.starttls.starttlsClient)
- description and source-code
```javascript
function starttlsClient(socket, options, callback) {
  return starttls(socket, options, callback, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ftpd.starttls.starttlsServer"></a>[function <span class="apidocSignatureSpan">ftpd.starttls.</span>starttlsServer (socket, options, callback)](#apidoc.element.ftpd.starttls.starttlsServer)
- description and source-code
```javascript
function starttlsServer(socket, options, callback) {
  return starttls(socket, options, callback, true);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)

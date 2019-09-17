# python-es6-server
A tiny python server for serving es6 javascript modules with support for handling request for extensionless js and correct mime types.

Trying to run a buildless environment using vanilla js and es6 modules turns out to be a bit tricky. 
This python server gets you some of the way there.
It supports:
- Serving your javascript files with the correct mime-type (because browsers actually care when you start using es6 modules)
- Serving your javascript files even when extensionless import syntax is used like ```import { foo } from "./bar"```

This server does not solve the problem of relative path hell and imports that choose to drop the leading slash.
For a full solution I am now using [es-dev-server](https://github.com/open-wc/open-wc/tree/master/packages/es-dev-server)

Anyway, if you do use this just download the python file and doubleclick it in the root directory you want to run the server from or run it with ```python startLocalWebserver.py```

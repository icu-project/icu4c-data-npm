WHAT IS THIS
===
[ICU4C](https://ssl.icu-project.org) data, now available via NPM.

Actually, instead of using this module directly, see [full-icu](https://www.npmjs.com/package/full-icu) instead,
and also [#3460](https://github.com/nodejs/node/issues/3460)

WHY DO I NEED THIS
===
See [node Intl docs](https://nodejs.org/api/intl.html) for more details

WHAT VERSION DO I NEED
===

run this:
```
node -e 'console.dir("npm install icu4c-data@"+process.config.variables.icu_ver_major+process.config.variables.icu_endianness)'
```

USE (example, replace l with b for big-endian)
===
```
npm install icu4c-data@54l
node --icu-data-dir=node_modules/icu4c-data -e "console.dir(new Date().toLocaleString('ru',{month:'long'})));"
```

LICENSE
===

- Usage of data and software is governed by the [Unicode Terms of Use](http://www.unicode.org/copyright.html)
a copy of which is included as [LICENSE](./LICENSE)

COPYRIGHT
===

Copyright &copy; 1991-2021 Unicode, Inc.
All rights reserved.
[Terms of use](http://www.unicode.org/copyright.html)

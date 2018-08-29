# dAPI.js

API for dApps on Ontology blockchain. It is an implementation of [OEP-6](https://github.com/backslash47/OEPs/blob/oep-dapp-api/OEP-6/OEP-6.mediawiki) communication protocol.



# Usage
dAPI.js can be used as CommonJS/ES6 module or directly referencing in web page html.

### Import CommonJS
```
var client = require('ontology-dapi').client;
```

### Import ES6 module
```
import { client } from 'ontology-dapi';
```

### Web require
The browser.js file under the '/lib' folder needs to be referenced from the page:
```
<script src="./lib/browser.js"></script>
```

The use of the code is required under the global namespace of Ont.
```
var client = dApi.client;
```

### Initialize

### Call

# Documentation

All the methods of dAPI from OEP-6 are organized into smaller units: **asset**, **identity**, **message**, **network**, **provider**, **smartContract** and **utils**.
The definitions of the methods can be found directly in the [OEP-6](https://github.com/backslash47/OEPs/blob/oep-dapp-api/OEP-6/OEP-6.mediawiki).

# Build

### Required Tools and Dependencies

* Node
* Npm

### Developing

Execute these commands in the project's root directory:

#### Download
```
git clone 'https://github.com/OntologyCommunityDevelopers/ontology-dapi.git'
cd ontology-dapi
```

#### Install

```
npm install
```

#### Development build
This will build the extension with minimum polyfilling for better debug experience.

````
npm run build:dev
````

You will get the packaged code under '/lib'.

#### Production build 

````
npm run build:prod
````

You will get the packaged code under '/lib'

## Built With

* [TypeScript](https://www.typescriptlang.org/) - Used language
* [Node.js](https://nodejs.org) - JavaScript runtime for building

## Authors

* **Matus Zamborsky** - *Initial work* - [Backslash47](https://github.com/backslash47)

## License

This project is licensed under the ISC License - see the [LICENSE.md](LICENSE.md) file for details

Lorem Ipsum Generator API
============

Lorem Ipsum Generator is a simple tool for generating lorem ipsum text. It returns the generated text.

![Build Status](https://img.shields.io/badge/build-passing-green)
![Code Climate](https://img.shields.io/badge/maintainability-B-purple)
![Prod Ready](https://img.shields.io/badge/production-ready-blue)

This is a Javascript Wrapper for the [Lorem Ipsum Generator API](https://apiverve.com/marketplace/api/loremipsumgenerator)

---

## Installation
	npm install @apiverve/loremipsumgenerator --save

---

## Configuration

Before using the loremipsumgenerator API client, you have to setup your account and obtain your API Key.  
You can get it by signing up at [https://apiverve.com](https://apiverve.com)

---

## Usage

The Lorem Ipsum Generator API documentation is found here: [https://docs.apiverve.com/api/loremipsumgenerator](https://docs.apiverve.com/api/loremipsumgenerator).  
You can find parameters, example responses, and status codes documented here.

### Setup

```
var loremipsumgeneratorAPI = require('@apiverve/loremipsumgenerator');
var api = new loremipsumgeneratorAPI({
    api_key: [YOUR_API_KEY],
    secure: true //(Optional, defaults to true)
});
```

---


### Perform Request
Using the API client, you can perform requests to the API.

###### Define Query

```
var query = {
  sentences: 3,
  words: 150
};
```

###### Simple Request (using Callback)

```
api.execute(query, function (error, data) {
    if (error) {
        return console.error(error);
    } else {
        console.log(data);
    }
});
```

###### Example Response

```
{
  "status": "ok",
  "error": null,
  "data": {
    "words": 150,
    "sentences": 0,
    "text": "deserunt aliquip duis pariatur nostrud cupidatat esse occaecat ea proident proident nulla labore eiusmod ut qui enim deserunt eu sunt ea ipsum et ullamco consequat ea laboris ea Lorem elit quis magna nulla mollit occaecat adipisicing aliqua reprehenderit nostrud laboris dolor magna sint ullamco Lorem eu commodo amet velit Lorem fugiat sunt Lorem culpa sit tempor laboris consectetur commodo et ipsum velit proident proident nostrud culpa irure consectetur non est minim commodo ullamco pariatur cupidatat exercitation ullamco in elit aliqua quis eiusmod tempor et nisi reprehenderit commodo duis consectetur excepteur occaecat labore ut mollit ipsum quis dolore est mollit mollit eiusmod id aliqua velit consectetur velit aliquip Lorem consequat et ad magna consectetur ad voluptate sunt dolore laboris mollit labore eu veniam non nostrud nostrud qui ex ad et aliquip ullamco ad consequat est velit non sunt ullamco non laborum aute fugiat cillum velit fugiat elit irure velit ex dolore"
  }
}
```

---

## Customer Support

Need any assistance? [Get in touch with Customer Support](https://apiverve.com/contact).

---

## Updates
Stay up to date by following [@apiverveHQ](https://twitter.com/apiverveHQ) on Twitter.

---

## Legal

All usage of the APIVerve website, API, and services is subject to the [APIVerve Terms of Service](https://apiverve.com/terms) and all legal documents and agreements.

---

## License
Licensed under the The MIT License (MIT)

Copyright (&copy;) 2024 APIVerve, and Evlar LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
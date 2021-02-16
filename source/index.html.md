---
title: Koi Protocol

language_tabs: 
  - javascript
  - shell

toc_footers:
  - <a href='https://discord.gg/nFXBAy6FXH'>Join the Discord Server for Help!</a>
  - <a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true

code_clipboard: true
---

# Tools for Easy Protocolization
pro·to·col
/ˈprōdəˌkôl,ˈprōdəˌkäl/

noun

the official procedure or system of rules governing affairs of state or diplomatic occasions.
"protocol forbids the prince from making any public statement in his defense"

# Tokenized Protocols
Bitcoin and others have popularized the system of using tokens within a network of peers as a means of rewarding good behaviour. This addition has expanded the feasibility of protocols as tools for social change, and specifically has created a new type of economic motive which can be sharpened and honed specifically for a particular task.

# Koi
The aim of the Koi network is to provide a convenient and simple way for software developers to easily concieve, implement, and deploy new mechanisms, while also enriching the public commons. 

Koi provides a suite of software tools designed to:
  1. Reward attention-based contributions, such as art and public data sets;
  2. Reliably track and reward repeatable tasks;
  3. Establish incentives and markets to reward profitable shifts in behaviour of (1) or (2).

---
# Join the Network
The Koi Network is made up of devices running compatible protocol software. Install the "Koi Tools" to join.

```javascript
const tools  = require('koi-tools')
const ktools = new tools()
const walletKeyLocation = "/path/to/your/wallet.json";

async () => {

    await ktools.loadWallet(walletKeyLocation)

    console.log('ktools', ktools)

}

```
```shell
$ npm i -g koi
$ koi init --key "/path/to/your/wallet.json"
```

> Make sure to replace `/path/to/your/wallet.json` with the location of your wallet file.

<aside class="notice">
You must replace <code>/path/to/your/wallet.json</code> with the path to a valid Arweave wallet file. 
</aside>

---
# Registering Content
Every 24 hours, the Koi Network votes to mint 1000 new tokens and awards them to the registered owners of the most popular content since the previous day. 

```shell
# With shell, you can just pass the correct header with each request
koi register "GoKkAKHi-g2WsVtcKKYqhRgpxOHlgtPRDxkIHC6FIAY" 
```

```javascript
let txId = 'GoKkAKHi-g2WsVtcKKYqhRgpxOHlgtPRDxkIHC6FIAY';

var result =  await ktools.registerData(txId);

console.log('transaction', result)
```

> Make sure to replace `GoKkAKHi-g2WsVtcKKYqhRgpxOHlgtPRDxkIHC6FIAY` with the address of the content you want to register.

<aside class="notice">
Be sure to replace <code>GoKkAKHi-g2WsVtcKKYqhRgpxOHlgtPRDxkIHC6FIAY</code>. This is the address of the <a href="https://dkbkiafb4l5a3fvrlnocrjrkqumctrhb4wbnhuipdeebylufeada.arweave.net/GoKkAKHi-g2WsVtcKKYqhRgpxOHlgtPRDxkIHC6FIAY">Koi Whitepaper</a>.
</aside>
<!-- 
# Kittens

## Get All Kittens

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```shell
curl "http://example.com/api/kittens" \
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2" \
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Delete a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.delete(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.delete(2)
```

```shell
curl "http://example.com/api/kittens/2" \
  -X DELETE \
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint deletes a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete
 -->

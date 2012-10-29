ooki Chip API (v0.0.1)

### URL

POST http://red.coo.ki/chips

### Requirement

* Sender must login in red.coo.ki.
* Sender must own Chips more than to send.


### DATA

name     | value
---------|------
user_id  | Cooki User's ID who will receive the chips.
site_uri | Uniform resource identifier
chips    | The amount of Chips.


### DEMO URL

http://red.coo.ki/dev/demo/chip


### Result Success
```
{
  "id":9165,
  "chips":"7.0",
  "from_user": { 
    "id":4,
    "name":"Siwon Choi",
    "image_thumb":"https://cooki-jp.s3.amazonaws.com/users/images/4/thumb/398769_2589222609734_433718147_n.jpeg?1346068708"
  }
}
```

### Result Failure
```
["OvenException::ChipLackError", "error2", ..]
```


# OpenHomeMatic

## Call Order

See [Postman Collection](source/postman/collection.json)

### Get SID (authenticate)
HTTP-POST: **http://192.168.178.43/api/homematic.cgi**
``` json
{
  "method": "Session.login",
  "params": {
    "username": "myusername",
    "password": "mypassword"
  }
}

```

### Get sensor value by sensor id
HTTP-POST: **http://192.168.178.43/api/homematic.cgi**
``` json
{
  "method": "Channel.getValue",
  "params": {
    "_session_id_": "mysessionid",
    "id": 1419
  },
}
```

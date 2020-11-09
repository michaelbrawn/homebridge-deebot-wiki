At the time of writing, the current LTS version of node.js is v14.15.0 as is the version I recommend to all users.

You will need to restart Homebridge/HOOBS after updating your version of node

### Homebridge

Please see the [How To Update Node.js](https://github.com/homebridge/homebridge/wiki/How-To-Update-Node.js) article on the Homebridge wiki.

### HOOBS

You can run this command in the HOOBS terminal to update your version of node:

```bash
wget -q -O - http://bit.ly/get-hoobs | sudo bash /dev/stdin --node lts
```
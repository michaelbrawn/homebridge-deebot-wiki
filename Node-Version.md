## Supported Node Versions

* The recommended version of Node to run Homebridge with is currently v14.17.3
* This plugin works with Node v12 and v14 - the versions of node that Homebridge officially supports
* This plugin should work with Node v10 and v16 - however Homebridge **does not** officially support these versions

## Updating Node

### Homebridge

* Please see the [How To Update Node.js](https://github.com/homebridge/homebridge/wiki/How-To-Update-Node.js) article on the Homebridge wiki.

### HOOBS v4

* You can use the 'Check for Updates' feature to update your Node version:

    ![hoobs 4 node update](https://user-images.githubusercontent.com/43026681/114992866-1f73dc80-9e93-11eb-9f4b-a511d1522d1e.png)

## HOOBS v3

Only do this if you are comfortable with accessing your HOOBS instance via SSH as in some circumstances this will be required.

1. Run this command in the HOOBS terminal to update your version of node:

    ```bash
    wget -q -O - http://bit.ly/get-hoobs | sudo bash /dev/stdin --node 14.17.3
    ```

2. Once this has finished it's a good idea to restart the HOOBS server
3. If the HOOBS UI becomes unresponsive, access your HOOBS instance via SSH and run these two commands separately:

    ```bash
    sudo npm uninstall -g @hoobs/hoobs
    sudo npm install -g --unsafe-perm @hoobs/hoobs
    ```

4. Once this is complete, the HOOBS UI should become available again with node updated. You can verify the system's version of node in the HOOBS terminal by running:

    ```bash
    node -v
    ```
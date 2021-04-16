## Supported Node Versions

* This plugin works with Node v10, v12 and v14.
* I recommend using Node v14.16.1 and if you are running an earlier version then you may receive a warning saying the plugin is incompatible (this is not the case as per the point above).
* The reason for displaying this warning is a helpful reminder that a newer version of Node is available and, for good practice, updating would be a good idea.

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
    wget -q -O - http://bit.ly/get-hoobs | sudo bash /dev/stdin --node 14.16.1
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
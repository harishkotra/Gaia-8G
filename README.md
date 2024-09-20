# Gaia-8G

### This is a quick guide if you're trying to run a node on a machine that doesn't meet the minimum system requirements as mentioned [here](https://docs.gaianet.ai/node-guide/quick-start/)

#### We highly recommend you run your own nodes on a machine that matches the [system requirements](https://docs.gaianet.ai/node-guide/quick-start/).

## Install the Gaia Node by running the command below

```
curl -sSfL 'https://github.com/GaiaNet-AI/gaianet-node/releases/latest/download/install.sh' | bash
```

![image](https://github.com/user-attachments/assets/1660586e-bda9-4a63-a7ad-4bd27f215a51)

Run the command printed on the terminal to set up the environment path, it is started with `source`

## Run the following command to update your `config.json` to run with a small language model.

```
gaianet init --config https://raw.githubusercontent.com/harishkotra/Gaia-8G/refs/heads/main/config_8g.json
```

## Run the node

```
gaianet start
```

A successful start prints a public URL for the node. Opening a browser to that URL will display the node information and allow you to chat with the AI agent on the node. 

Load the link printed at the end of the log (e.g., `https://0x1234...wxyz.us.gaianet.network`) in your browser or simply load `http://localhost:8080/`

## Monitor the log in the terminal

```
tail -f ~/gaianet/log/start-llamaedge.log
```

## To stop the node

```
gaianet stop
```

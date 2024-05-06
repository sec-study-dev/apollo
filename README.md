# Apollo


## Dataset
Our collection of all MEV transactions for 2023 can be found [here](https://drive.google.com/drive/folders/1Mt0DrXo9A1r-Elz08MkaFkTeomG9fC-W?usp=drive_link).

## Quick Start
To open the container, install docker and run:
```
docker pull secartifacts/apollo
docker run -it secartifacts/apollo
```

To evaluate a simple contract inside the container, run:
```
python main.py --iden-builder 0x93FFb15d1fA91E0c320d058F00EE97F9E3C50096
```
and you are done!

## Running Instructions
```
 █████╗ ██████╗  ██████╗ ██╗     ██╗      ██████╗ 
██╔══██╗██╔══██╗██╔═══██╗██║     ██║     ██╔═══██╗
███████║██████╔╝██║   ██║██║     ██║     ██║   ██║
██╔══██║██╔═══╝ ██║   ██║██║     ██║     ██║   ██║
██║  ██║██║     ╚██████╔╝███████╗███████╗╚██████╔╝
╚═╝  ╚═╝╚═╝      ╚═════╝ ╚══════╝╚══════╝ ╚═════╝ 


usage: main.py [-h] [--iden-builder IDEN_BUILDER] [--iden-catalyst {False,True}] [--death {arbitrage,sandwich,liquidation}] [--bot-builder {False,True}] [--builder-analysis {False,True}] [--catalyst-analysis {False,True}] [--sender-bot-type {arbitrage,sandwich,liquidation}]
               [--sender-analysis {False,True}] [--token-bot {arbitrage,sandwich,liquidation}] [--token-bot-type {arbitrage,sandwich,liquidation}] [--archive-node ARCHIVE_NODE] [--rpc-host RPC_HOST] [--rpc-port RPC_PORT]

optional arguments:
  -h, --help            show this help message and exit
  --iden-builder IDEN_BUILDER
                        Identify the builder of each transaction of a bot.
  --iden-catalyst {False,True}
                        Identify catalyst transactions.
  --death {arbitrage,sandwich,liquidation}
                        Analysis of dead bots.
  --bot-builder {False,True}
                        Analyse the builder distribution for each bot.
  --builder-analysis {False,True}
                        Analyse the builder distribution of transactions for all bots.
  --catalyst-analysis {False,True}
                        Analyse catalyst transactions.
  --sender-bot-type {arbitrage,sandwich,liquidation}
                        Analyse the transaction initiation strategies for each type of bot.
  --sender-analysis {False,True}
                        Analyse transaction initiation strategies.
  --token-bot {arbitrage,sandwich,liquidation}
                        Analyse the tokens involved in each bot.
  --token-bot-type {arbitrage,sandwich,liquidation}
                        Analyse the tokens involved in each type of bot.
  --archive-node ARCHIVE_NODE
                        Ethereum archive node address.
  --rpc-host RPC_HOST   Ethereum client RPC hostname.
  --rpc-port RPC_PORT   Ethereum client RPC port.
```


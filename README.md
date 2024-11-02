# Solcrates Bot 🤖
❓ **What is exactly a Solcrates Bot?** ❓

🤖 **Solcrates Bot is an automatic algorithmic trading system on SOL chain for trading memecoins and other on-chain coins, that runs locally on your computer/VPS, and uses live OHLCV data, creating tech-analysis algorithms that allow you to auto-trade exactly as the strategy sounds, providing you with good automatic profit-take/stop-loss.**

Some strategies allow you to run it 24/7 without taking a look on logs, but we do not recommend that.(at least on beta version)


## How do we start?
For now, Solcrates Bot is a closed-source project. You need to download it from the RELEASE section of the repository as a executable file, listed in the right-middle section of the repository page. As the program is already precompiled file, you don't need to download NodeJS and modules to use it.

### For Windows
Download .exe from releases of solcratesbot repository and launch it

**OR**

Use curl to download the release
cd into your custom folder or make the new folder

```
mkdir solcratesbot
cd solcratesbot
curl -L https://github.com/Solcrates-Labs/solcratesbot/releases/download/v0.1.0-beta-fixed/solcratesbot-win.exe > solcratesbot-win.exe
```

### For Linux
**Use wget or curl**

**If you use wget**

```apt install wget```

Create a folder for program, then with wget you now need to download the latest linux release of the bot

```
mkdir solcratesbot
cd solcratesbot
wget https://github.com/Solcrates-Labs/solcratesbot/releases/download/v0.1.0-beta-fixed/solcratesbot-linux

IF YOU USE CURL REPLACE WGET with
curl -L https://github.com/Solcrates-Labs/solcratesbot/releases/download/v0.1.0-beta-fixed/solcratesbot-linux > solcratesbot-linux
```

To run a program after installation

```
chmod +x solcratesbot-linux // Execute this once to make solcratesbot-linux an executable
./solcratesbot-linux
```

❓ **As the program starts, it will create .env file for environmental variables(stored only on your PC/VPS) to list in:
Private_key variable: The private key of your solana wallet.
Rpc_url variable: Remote Procedure Call URL. You can get it from diverse RPC Solana providers, such as Helius, Alchemy, Quicknode, GetBlock, PublicNode. Usually free/freemium tier is enough to run a program if you use only basic strategies that are not SCALPING and ARBITRAGE**

After setting all variables in .env file, launch program again.

✔️ After launching, you can set all desired options to trade in program in a user-friendly command line interface. These options include:

1.) Strategy: The strategies to use with a quick info, pros/cons about them.

2.) Buying token: What token will be used to buy? Supports stablecoins and popular solchain coins. (for now)

3.) Trading token: What token will be speculated on? Supports only jup strict-list tokens for safety measures.(for now)

4.) Trading amount: Trading amount per transaction in USD?

5.) Global stop-loss percent number.

6.) Slippage percent number.(Auto converts to BPS)

7.) Priority Fee Max lamports.(Very important setting, it may highly impact your trading performance)

8.) Sending transaction cooldown in milliseconds number(If your RPC gives your **TOO MANY REQUESTS 429** errors, you need to make it higher)

9.) Use Field-testing(debug) mode(Will replace trading amount you set before with 0.01 usd)

__Note: Good for RPC testing, but Priority fee number won't be changed.__

**After setting everything up, you confirm it and the program starts trading. For beta version logging and trading interface is still blunt, but it will be updated in the next versions of the program.**

***You're good to go.***

## Post Scriptum
### DISCLAIMER
❗ ***This program must be used with second, 'burner' wallet to perform trading/transactions. The author of the program is not responsible for actions of third party that may lead to loss of their funds from using the program. Profit is not guaranteed while using the program, the program is a TOOL and must be used as a TOOL. Responsive usage of the program is highly advised. This program uses progressive fee system for each trading deal, when the fee is being taken only in one circumstance: if the trading deal is profitable. Note that the program is still in development and you may encounter 'bugs' or other software-related errors.*** ❗

### GLOBAL NOTE 
❗ ***SOLCRATES BOT IS NOT INTENDED FOR USE IN LIVE NEW PAIRS! Solcrates Bot is a speculating trading bot, not a sniper/arbitrage(at least not yet) bot. It can be used efficiently only under certain circumstances, which usually imply that the coin you trade IS AT LEAST MONTH OLD and it is already grown of the decent community and doesn't have high volatility! That does not mean you can't experiment, Solcrates Bot is a TOOL and can be used in whatever way you like, just remember that profit is not guaranteed.*** ❗

### Bugs and errors 🐞
**While using Solcrates Bot Beta you may encounter bugs and different errors due to development. Please reach out on our Discord or Github Issues of this repo to provide further information about the issue.**

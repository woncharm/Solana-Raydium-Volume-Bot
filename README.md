# Raydium Volume Bot

This volume bot distribute SOL to multiple wallets and buy and sell with that distributed wallets permanently on the Raydium platform.

## Features

- **Automated Wallet Creation**: Create number of wallets automatically to buy and sell the token
- **Automated SOL Distribution**: Distributes SOL to those new wallets.
- **Endless Buy and Sell Swaps**: Buy and Sell with those wallets permanently.
- **Configurable Parameters**: Allows customization of buy amounts, intervals, distribution settings, and more.

## Usage
1. Clone the repository
```
git clone https://github.com/sourlodine/Solana-Raydium-Volume-Bot.git
cd Solana-Raydium-Volume-Bot
```
2. Install dependencies
```
npm install
```
3. Configure the environment variables

Rename the .env.example file to .env and set RPC and WSS, main wallet's secret key, and jito auth keypair.

4. Run the bot

```
npm run start
```


## Specific Features
- ✅ **Transferring SOL to new wallet**: After buying and selling in one wallet, it transfers SOL to a newly created wallet and continues buying and selling there.
- ✅ **Maker increase**: New wallets are created every round of buying and selling, increasing the number of makers.
- ✅ **Sell before gather**: When gathering, if there are tokens left in the wallet, it sells the tokens first and gathers only SOL (the token account rent of 0.00203 SOL is reclaimed).
- ✅ **More buys than sells**: It randomly buys twice with SOL in the wallet and sells all tokens after some time, making the number of buys twice as many as sells, thus creating more buy pressure.

## Contact me if you have question

[Telegram](https://t.me/evilgon_dev)

## You can always feel free to find me here for my help on other bots like Raydium sniping bot, Shit-token Launcher, Token-freezer, Pumpfun sniper, Market making bot.

# What is TokBot?

TokBot is a tip bot made to distribute the Ethereum-based ERC20 cryptotoken, 🅱️itcoin, on reddit.

# How do I get 🅱️itcoin?

You can acquire 🅱️itcoin in two ways:

- Redeem: **Redditors who submitted to /r/dankmemes before August 12th, 2017 can redeem 1 million 🅱️itcoin**. To do this, use the 'redeem' command as described below. Up to 50 Billion 🅱️itcoin can be redeemed by redditors.

- Tip: Users of /r/dankmemes can tip 🅱️itcoin to each other using the tip command described below. If someone tips you 🅱️itcoin, you will immediately have the pills available to tip others on reddit.

# How do I interact with the bot?

TokBot responds to the following public command in comments posted to /r/dankmemes.

* u/tokbot tip [amount] 🅱️itcoin (ex: u/tokbot tip 5000 🅱️itcoin)

The above command sends a tip of 5k 🅱️itcoin to the author of the comment or post you're responding to. You must have a balance above or equal to the amount of 🅱️itcoin you would like to tip

You can send tokbot a private message with the following private commands:

* balance 🅱️itcoin (ex: balance 🅱️itcoin)
* redeem 🅱️itcoin (ex: redeem 🅱️itcoin)
* confirm [address] (ex: confirm 0x9901c66f2d4b95f7074b553da78084d708beca70)

# How do I withdraw 🅱️itcoin?

You can withdraw your 🅱️itcoin to any ethereum wallet that supports ERC20 tokens. In order to do so you need to set up a watch contract in your wallet with the following info:

    Token address: 0xF5afDF8Bf72e292107a18dAcF88dAa6831334Ad1
    ABI:

After setting up the watch contract, you'll need to confirm your withdrawal address with the tipbot. To do so, send a private message with the command 'confirm'

* confirm [address] (ex: confirm 0x9901c66f2d4b95f7074b553da78084d708beca70)

After confirming your withdraw address, use your Ethereum wallet to call the RequestWithdraw function from the contract. Include your reddit name, the amount you'd like to withdraw and send at least 0.005 ETH with the withdraw request transaction. The withdrawal request must be sent from the address you have confirmed with the confirm command.

The small amount of ETH is used to cover the cost of the withdrawal transaction. If you do not include the ETH fee, your withdraw request will not be approved.

# How do I deposit 🅱️itcoin?

If you aquire 🅱️itcoin outside of reddit you can deposit them into your reddit tipbot account by interacting with the smart contract directly. To do so, first set up a watch contract for 🅱️itcoin in your ethereum wallet using the following info:

    Token address: 0xF5afDF8Bf72e292107a18dAcF88dAa6831334Ad1
    ABI:

Then use the Deposit function on the 🅱️itcoin contract with your reddit name and the amount to deposit. Deposits will be processed periodically and will appear in your tipbot account when successfully confirmed.

Note that 🅱️itcoin received on reddit via the redeem or tip commands will appear in your balance instantly once processed.

-------

*Disclaimer: TokBot is beta software and should be treated as such. The owner of TokBot reserves the right to terminate the reddit bot service at any time, for any reason. Do not store large amounts of 🅱️itcoin on the tipbot wallet. 🅱️itcoin can be withdrawn to a local ethereum wallet on your computer using the steps described above. TokBot is not responsible for the 🅱️itcoin stored on it's servers.

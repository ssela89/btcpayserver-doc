# Deploying BTCPay - LunaNode Web-Wizard

This article explains the deployment of BTCPay Server through LunaNode Web-Wizard. [LunaNode](http://lunanode.com/) is Canadian based hosting provider that accept Bitcoin payments and requires no personal identification except for a phone number verification.

Their web-wizard is one of the easiest ways to deploy BTCPay Servers from a very user-friendly interface. This method is highly recommended if you do not have any technical knowledge. For the price of around US$ 8.8 per month, you can have a self-hosted BTCpay, which includes a Bitcoin full node and Lightning Network node.

Video bellow explains all the step and customization of BTCPay.

[![LunaNodeWebWizzard](https://img.youtube.com/vi/NjslXYvp8bk/mqdefault.jpg)](https://www.youtube.com/watch?v=NjslXYvp8bk "BTCPay - LunaNode Web-Deployment")

The instalation is also covered in [this article](https://medium.com/@BtcpayServer/launch-btcpay-server-via-web-interface-and-deploy-full-bitcoin-node-lnd-in-less-than-a-minute-dc8bc6f06a3)

The third video covers setting BTCPay up on LunaNode, but also goes in-depth on setting up wallets, store and apps.

[![LunaNodeWebWizzard2](https://img.youtube.com/vi/00YCc87RwnU/mqdefault.jpg)](https://www.youtube.com/watch?v=00YCc87RwnU "BTCPay - LunaNode Web-Deployment Video")

## 1. Create the account and add credits

Register to LunaNode and add credits to your account. The process is quite straight-Forward. If by any chance you get stuck, [see this article](https://bitcoinshirt.co/how-to-create-store-accept-bitcoin/8/#Creating-an-account). Wait for your invoice confirmation.

## 2. Create the API Key

Once your account has been verified, and credits added, go to the API section and create a new API. Do not close that page and proceed to step 3.

## 3. Web-Wizard Deployment

1. Go to [launchbtcpay.lunanode.com](http://launchbtcpay.lunanode.com/)
2. Paste the API Key and API ID created in step 2. and continue.
3. Use your own domain or automatically-generated one by LunaNode.
4. Customize the web-wizard settings according to your needs.
5. Click Launch VM. Wait 6-7 minutes for Virtual Machine deployment.
6. Visit the domain.

Now you need to wait for blockchain to sync fully. Depending on the plan you used and the number of coins you added, that can take 1-7 days. If you enable CPU utilization, with Bitcoin and LND, it will take 3 days. There is a US$ 3 one-time charge for faster sync if you enable the CPU utilization. The sync pop-up window will disappear when your node fully syncs.

Note: During installation a ssh user is created. This allows you to access your VM after the installation process (for details how to connect see [SSH Lunanode](https://github.com/JeffVandrewJr/patron/blob/master/SSH.md) ). Please note that this is a **potential security risk**. It is advised that you change at least username and password (both!). For better security you should generate a private-public key pair for ssh access. A tutorial can be found here [Tutorial](https://github.com/ssela89/master/blob/master/ssh_btcpay_private_public_key.md) .

# Node-RED_TranaslationBot-Dutch-English

Node-RED translation bot using the IBM Node-RED Starter with the services Language Translator, Speech to Text and Text to Speech.

## Getting Started
Perform the following steps to make your own translation bot

### Prerequisites
To complete the translation bot, you need the following artifacts:

*	Obtain an **IBM Cloud** account.
*	Provision the **Language Translator** service
*	Provision the **Language Identification** service
*	Provision the **Speech to Text** service
*	Provision the **Text to Speech** service
*	Provision the **Node-RED starter** app
*	Install **Telegram** app on your device

### Step 1. Create Telegram bot
After installing Telegram on your device, search for "BotFather"
After you find it, send a `/newbot` command and follow these instructions:
1.	Set a name.
2.	Set a username. 
3.	Save the access token for future use

### Step 2. Create a Node-RED flow
1.	Go to your **IBM Cloud** account and click **Catalog.**
2.	Choose **Starter Kits** from the left menu.
3.	Select **Node-RED Starter**, as shown in the following figure.
4.	Complete the fields to create the app:
    * **App name:** Must be unique in the IBM Cloud domain.
    * **Host name:** Is filled out automatically based on the App name.
5.	Click **Create.**
6.	Wait for a few seconds until the application shows Running, then click **Visit App URL.**
7.	Enter a username and password, selecting the option to secure your profile so that only authorized users can access it.
8.	Click **Go to your Node-RED flow editor.**

### Step 3 Connecting IBM services
Before we can start configuring our bot we need to link the IMB services to the Node-RED application.

1.	Go to the Node-RED application in IBM Cloud and click the **Connections** tab in the left menu. Click **Create connection**
2.	Connect all of the required services. (See Prerequisites)
3.	Restage the app to configure the new changes.

### Step 4. Configure the Telegram bot
Once in the Node-RED flow editor:
1.	Select **Manage palette** from the upper right menu.
2.	From the Manage palette menu, click the **Install** tab then search for telegram.
3.	Install **node-red-contrib-telegrambot** and close the palette menu.
4.	Copy the code from the Node-RED-flow.json file and import it into the Node-RED clipboard.
5.	Double-click the Telegram receiver node and click the pencil icon for configuring your bot credentials.
6.	Complete the Bot-Name (username from 1.1) and Token fields according to the bot credentials that you created earlier.
7.	Click **Update.**
8.	Double-click the Telegram sender node, select the bot credentials that you created in the Telegram receiver node and click **Done**
9.  Click **Deploy**

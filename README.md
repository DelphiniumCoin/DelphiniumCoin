# Delphinium Coin: P2P Cryptocurrency without need of historical operations.  
  
Copyright (c) 2018 DelphiniumCoin
  
THIS IS EXPERIMENTAL SOFTWARE. 
  
This software is a Node of the Delphinium Coin P2P Cryptocurrency.  
It can be used to Mine and Explore blocks and operations.  
  
This product includes software developed by the OpenSSL Project and Denis  
Grinyuk (https://github.com/Arvur/OpenSSL-Delphi), and some  
cryptographic functions inspirated in code written by Ladar Levison and   
Marco Ferrante. 
This product includes software developed by the PascalCoin project:
https://github.com/PascalCoin/PascalCoin

## How to download Delphinium Coin:

Open your favorite webbrowser and surf to:

https://github.com/DelphiniumCoin/DelphiniumCoin

Navigate to the latest version folder, currently version 3.0.1.1

Then either download the *.rar file or the *.zip file based on your preferred compression technology (winrar) or (winzip or zip build into windows 7) (from the version folder).

For example:

DelphiniumCoinVersion3.0.1.1.zip

## How to install:

Extract the compressed file (DelphiniumCoinVersion3.0.1.1.zip) to a folder on your preferred drive and folder for example:

C:\Tools

After extraction the following main subfolder will exist:

C:\Tools\DelphiniumCoin

## How to run:

Navigate to this folder using Windows Explorer (a folder exploration tool of your windows operating system).

Then navigate to the "Wallet" folder.

Now navigate to either the 32 bit or 64 bit version folder matching the bitness of your operating system.

Example:

C:\Tools\DelphiniumCoin\version 3.0.1.1\Wallet\32 bit version\

When in doubt simply run the 32 bit version (DelphiniumCoinWallet32bit.exe), though it is advisible to run the 64 bit version (DelphiniumCoinWallet64bit.exe).

(The last part .exe may be hidden best on your windows explorer preferences).

## How to install initial blockchain

This step can be skipped if DelphiniumCoin connects to other Peers and downloads the blockchain from them.

However if no peers are available it's still possible to mine by installing the blockchain yourself.

This is recommended for "network boot up" in case then network is still small or divided.

Be warned though, mining on a disconnect blockchain is risky, once connected the blockchain with the most work will win and thus

if your local blockchain is weaker/less work performed it will be replaced.

To install the blockchain start the wallet and go to project->options at the bottom there will be a button called "open data folder".

Click on this button.

The data folder will look similiar to the following:

C:\Users\<Your windows username>\AppData\Roaming\DelphiniumCoin

Close the wallet, make sure it's terminated by checking task manager, hold control-shift-escape to bring up task manager, after a few seconds the wallet should disappear
if not right click on it and choose end process tree.

Inside this folder there will be a data folder for example:

C:\Users\<Your windows username>\AppData\Roaming\DelphiniumCoin\Data

Copy the contents of the "data" folder from the distribution/zip file into this data folder above.

Now restart the wallet, this should load the first few blocks and accounts that were mined.

Now the blockchain has a valid start and can be mined by anyone !

## How to add peers to the peer list:

Other people's computers (called peers) can be added to the network via the peer list. This allows their computers to be found and connected too.

The process of adding peers is quite easy:

In the wallet navigate to project->peer list.

A form will appear with a white box which should say:

delphiniumcoin.chickenkiller.com:4100

This is the default DNS name for the default peer, which will resolve to some IP address, the port is also added just in case though is not required and the default port will
be added automatically inside the software if omitted.

Any DNS or IP address running DelphiniumCoin can be added to the list by simply adding the new address on a new line for example:

delphiniumcoin.chickenkiller.com:4100
<your neighbours internet address>
<your mother's internet address>
<something special>:<port>

For example:

delphiniumcoin.chickenkiller.com:4100
212.23.23.124
34.23.32.65
43.65.232:6000

The port number can be specified in case delphiniumcoin needs to run on a different port on other computers.

## How to run the miner:

Go Delphinium main folder for example:

C:\Tools\DelphiniumCoin

There will be a subfolder called: "Miner" navigate to it.

Then navigate to the 32 bit version folder.

It is advisible to first edit RunMiner.bat with edit command, then change "YourUserName" to something more appriorate, though this is not mandatory.

Then run RunMiner.bat

(OpenCL will need to be installed for now, check websites of intel/nvidia/amd for OpenCL drivers)
 
Enjoy Delphinium Coin!
  
## Contact:

If you would like to contact the main developer of Delphinium Coin the e-mail address is: DelphiniumCoin@outlook.com

## History:  

### Version 3.0.1.1 created on 21 oktober 2018
+ PeerList added to application to allow users to create/setup their own networks.
+ Server port restriction relaxed a bit, now DelphiniumCoin should be able to run on different ports if required and can be connected to successfully by other peers and propagated (?).
+ Blockchain/Safebox data files added so users can setup the blockchain/safebox themselfes instead of downloading it from others in case others are not online yet, this allows
  booting/creation of the network.
- version 3.0.1 removed.

### Version 3.0.1 created on 16 oktober 2018 based on PascalCoin Build 3.0.1
+ Initial Launch
+ Inactivity period for accounts and coin recycling increased from 4 years to 200 years.
+ 64 bit safe arithmetic used for balances.


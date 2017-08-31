## Miner Network Operations
### Prupose
With the expanding field of crypto-currency, and subsequent rise in both individual and company mining operations, keeping track of all mining activity within a network can become difficult and complex. What's most important to those involved in the operation, however, is that the machines are mining as expected and the the currency is transferred to the right location. An ideal solution should track the crypto-currency during each step of it's journey, which begins when it is mined and ends when it reaches the owner's wallet.

The project accomplishes this using NetMon to identify the crypoto-currency being mined as well as it's destination by examining and filtering network packets. This allows the user to ensure that their mining operation is running correctly and quickly identify when a system gets interrupted so they can react accordingly.

First the packets are filtered so that only those originating from a mining computer are examined by checking the source IP. Next the packets are filtered to select only those running through the mining platform, in this case MinerGate by checking the application ID. The specific type of crypto-currency is then identified by the port number of it's packets, since each type has a unique port. This can be seen on the pie chart visualization which separates crypto-currency type by bandwidth allowing the user to monitor the type and amount of each currency being mined. 

Since the user would also like to ensure that the currency mined is arriving at the correct wallet, packet transactions including the MinerGate application ID, and again separated by port number are tracked to show interaction with each type of crypto-currency's wallet. This is displayed on an outer pie chart allowing the user to ensure that the same amount of currency that is mined, also arrives at a wallet of the same type.

In addition a series of currency specific graphs show the network activity for each type being mined, in this case, Etherium, Monero, and Dashcoin, identified using the transaction port number associated with each type. 
### Manifest
MinerSearches.json

MinerVisualizations.json

MinerDashboards.json

pcaps_2017_08_30_13_53_56.zip

pcaps_2017_08_30_13_55_05.zip

readme and screenshots

### Dependencies
This project was build to examine mining activity using the MinerGate mining console and has only tested using the MinerGate platform.
### Setup
Load MinerSearches.json to import all searches used within the project.

Load MinerVisualizations.json to recreate all charts and graphs displayed on the dashboard.

Load MinerDashboards.json for a complete dashboard for monitoring the operation of a mining network.

Test the project by uploading data one of the included pcap files to analyze data from our own mining network.
![Miner Network](https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/529/625/datas/gallery.jpg "Miner Network")
![Miner Network](https://challengepost-s3-challengepost.netdna-ssl.com/photos/production/software_photos/000/529/639/datas/gallery.jpg "Miner Network")

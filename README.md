# We will learn how to start alvinet for ZBank
First, you should git pull/download this file and we will start from there.

# Step to use Alvinet
1.
- open gitbash
- cd to POA-Development-Chain > ZChain
- Run below command
```
./geth --datadir node1 --unlock "6FDDe64b73b1240B6B59cfb90972d55C16B453Da" --mine --rpc --allow-insecure-unlock
```
```
./geth --datadir node2 --unlock "E5f9F696003354FE406Dc5F129264A914C3769C1" --mine --port 30304 --bootnodes "enode://0f692f5fd0c03142a42fe052d52c116bb74617d5afbb3cd09742241da239cd4bbf1ce441ee7b8e3d7b4352d8b40f29db6d252a2e6234f53daf2bba0eaadbe223@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock
```
Run the nodes in separate terminal windows with the commands.

there is no password.

2. 
Now open MyCrypto, Open the MyCrypto app, then click Change Network at the bottom left.

3.
Click "Add Custom Node", then add the custom network information that you set in the genesis.

4. Set network as Custom; Currency as ETH; chain id is 666; node name and network name is ```Alvinet```; URL is http://127.0.0.1:8545

5.
After connecting to the custom network in MyCrypto, it can be tested by sending money between accounts.

6.
Select the View & Send option from the left menu pane, then click Keystore file.

7.
On the next screen, click Select Wallet File, then navigate to the keystore directory inside your Node1 directory, select the file located there. there is no password so it would unlock by self.

8.
In the To Address box, type the account address from Node2, then fill in an arbitrary amount of ALVZ.

9.
Confirm the transaction by clicking "Send Transaction", and the "Send" button in the pop-up window.

10.
You should see the transaction go from Pending to Successful in around the same blocktime you set in the genesis.

You can click the Check TX Status button to update the status.
![Successful transaction](POA-Development-Chain\ZChain\Screenshots/tx.png)



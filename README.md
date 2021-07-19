# Unit 20 - "Looks like we've made our First Contract!"

## Objective: 

Create 'Associate Profit Splitter' contract that accepts ether into the contract and divides the Ether evenly among the associate level employees.

## Step 1:

Open Remix and write the contract code as per the screenshot, and  compile to make sure there are no errors:

![](images/1-compiled.png)

## Step 2:

Open Ganache and identify wallet addresses that will be used as payer and payees.  Observe their initial balances.  I have used address 0x3Ce1d05E5ADE55e24CA9eF6c03bC5DBd681760Bb as the payer.  It has an initial balance of 43.53 ETH.

I have used addresses 0x279184EcfeEd2506A8Da63E0D6087aC4C247026E, 0x56FC51014b3116f159D79DA52Fab912D187A5d6b, and 0xB46132ECbB8279e7E43758ac188a43fc4343EDe0 as the payees.  They all have initial balances of 100 ETH.

![](images/2-initial-ganache-balances.png)

## Step 3:

We are now ready to deploy the contract.  To do this, go to the deploy section in Remix, and enter in the payee addresses into the 3 inputs in the deploy section, then click 'transact':

![](images/5-deploy.png)

## Step 4:

In Ganache, observe the new block that has been mined for the contract deployment.  Also observe the new transaction that has been created as well:

New block for contract deployment

![](images/6-contract-creation-block.png)

New transaction for contract deployment

![](images/7-contract-creation-transaction.png)

## Step 5:

In Remix, we will now perform a deposit using this newly deployed contract.  I decided to deposit 9 ETH from the payer to the 3 payee addresses.

![](images/8-deposit.png)

## Step 6:

Go back to Ganache to observe the newly mined block and transaction for the deposit:

New block for deposit

![](images/9-deposit-block.png)

New transaction for deposit

![](images/10-deposit-transaction.png)

## Step 7:

In Ganache, observe the updated balances for the payer and payee addresses.  As you can see, the payer address balance has decreased by 9 ETH, and each of the payee address balances has increased by 3 ETH:

![](images/11-deposit-balances.png)



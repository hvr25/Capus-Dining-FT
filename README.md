# Capus-Dining-FT

This project is an implementation of ERC20 tokens with a web application including a wallet-MetaMask that delivers this token and lets
participants use it for the designated purpose. Implementation is divided into two parts: App and Contract

App: Consists of UI implemented using Node.js. The functions of Smart Contract are accessed through the UI.

Contract: Consists actual implementation of the Smart Contract and the corresponding functions

## Instructions for deploying:
1. Navigate to CDS-Dapp directory from terminal/command prompt
2. Go to CDS-Dapp>cds-contract and run truffle migrate –reset command. Note that you will have to have Ganache running in the back. This will compile and deploy the smart contract in your local.
3. Navigate to CDS-Dapp>cds-app and run the following commands

     Npm install

    Npm start
    
This will deploy js node.

4. Open web browser and use Ganache mnemonic to connect Metamask with Ganache network and accounts.
5. Open http://localhost:3000/ to view and access the UI part of the project.

## Running and testing the application: CDS-DAPP s

Feedback:

1. Choose any account other than owner. Enter 6-digit UB person number and click on Register.
2. Repeat the step to register multiple accounts.
3. Initially the balance is 0 (you can check this by clicking on Balance button). Now enter a rating in the feedback field and click on Feedback. You will then be rewarded with 10 CFB points.
4. In order to prevent students from misusing the system and providing multiple feedbacks to get points, timestamp is noted to make sure that only one feedback can be given per day. (For the purposes of demonstration, the time delay has been reduced from 24hrs to 100secs).
5. Now check the balance, there is a reward of 10 CFB tokens into your account.
6. Once you have sufficient tokens, you can redeem them for items with the respective amount.
7. Enter the item number in the redeem text field and click redeem.
8. Now if you check your balance, you will see deducted amount.
9. You can unregister yourself anytime by just clicking unregister button.
10. Additionally, the chairperson (contract deployer) can reward students by selecting the student’s address and clicking on reward.

Poll:

11. At any point, the chairperson can initiate a poll using the Initiate voting button.
12. After initiating, students can register for voting using the Register for Voting button.
13. The chairperson will have to then change the state to Vote(2).
14. In Vote state, all registered members/accounts can vote for their desired choice.
15. After all accounts have completed voting, the chairperson will have to then change the state to Result(3).
16. In Result state anyone can click on the Declare Winner button to see who has got the maximum votes


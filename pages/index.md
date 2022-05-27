# RomaN
<img src="submission.png" alt="submission" width="600"/>

## Description
RomaN is a 
    dating decentralized application,
    prepaid,
    pay by click,
    earn,
        built with 
            trust
            transparency
            honesty 
        in mind.

The blockchain comes with brilliant solutions to leverage web2 dating industry.

## Problem
Nowadays web2 dating applications have several problems :
    1. privacy 
        - web2 dating compagnies own users data like email, bank account information
    2. charges 
        - user have the choices between limited services or automatic monthly subscription via bank or PayPal and there is  hundreds of dating site per country.
        - There is few dating web2 sites lying on ads for monetizing , all functionalities are free to all users, but they are often full of spams and fake profiles.
    3. trust transparency
        - web2 site are full of bots and spam.

## Solution
At RomaN we analysis these problems and leverage the web3 technology to find solutions.
    1. privacy
        - on the blockchain users own their data
        - 
    2. charges
        - RomaN is designed to solve all the web2 monetisation problems.
            - Browse, search and filter profiles is free.
            - to create a profile, user have to mint a free* RomanToken an ERC721 token.
            - RomanToken is a SoulBound NFT. any address can mint only one token and transfer functions are blocked. 
            - RomanToken holders can deposit any value they want in stableCoin** to the RomanTokenVault contract(payment channel).
            - Interacting with others (view a profile***, like, msg, .....) will trigger a transfer of a variable amount of the stableCoin with no fees.
            - users can withdraw any time their sold or recharge their balance.
        - the site is ads free, we monetise by taking a percentage of the transfer to pay for the infra (hosting, ...) and the RomaN Team.
    3. trust transparency
        - all transactions are saved on the blockchain ledgers.
        - proof of humanity to mint a RomanToken - not implemented yet
        - verified users get bonus -  not implemented yet
        - Behaviour: transfer amount = amount*(behaviour/100) - charges
            - We assume all users are honest, when a user mint an RomanToken behaviour is set to 100 
            - each time a user get reported, behaviour is deducted by one which will affect directly 
            example: view profile = 100,
                     charges = 10,
                     user A behaviour = 100,
                     user B behaviour = 50 (user B blocked 50 times)
            user A view user B profile : user A pay 100, user B receive = 100*(50/100) - 10 = 40
            user B view user A profile : user B pay 100, user A receive = 100*(100/100) - 10 = 90

* plus tx fees
** using ether for testnet
*** some interactions are paid once

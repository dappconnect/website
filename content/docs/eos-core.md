# EOS Core


## Get Active Account

Returns the active account. Can be null if no account available or active.

/eos-core/get-active-account

## List Accounts

Lists all accounts associated with the wallet

/eos-core/list-accounts

## Transaction

/eos-core/transaction

## Remove Account

Removes the account from the list of available accounts. It also removes the private key.

/eos-core/remove-account


    {
        account: string
    }

## Transfer EOS

Transfers an EOS amount from the currently active account to the account specified.

/eos-core/transfer-eos
    {
        toAccount: "martinsunset"
        amount: "0.0001"
        memo: "Transfer"
    }

## Tansfer

Transfers a token within a contract from the currently active account to the account specified.

/eos-core/transfer

    {
        contract: "eosio.token",
        symbol: "EOS",
        toAccount: "martinsunset"
        amount: "0.0001"
        memo: "Transfer"
    }

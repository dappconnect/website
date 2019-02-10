# EOS UX

## Import Account

Opens up a modal screen that allows the user to import a private key, which, if successful, fetches all the accounts associated with it.

IN -> /eos-ux/import-account
OUT <- /eos-ux/import-account-success
OUT <- /platform/ux-user-cancelled

## Select Account

/eos-ux/select-account
OUT <- /eos-ux/select-account-success
OUT <- /platform/ux-user-cancelled

## Show Private Key

/eos-ux/show-private-key
OUT <- /platform/ux-user-cancelled
OUT <- /platform/ux-user-closed

## Show Explorer

/eos-ux/show-explorer

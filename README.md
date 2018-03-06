# TenancyDeposit
Welcome to the "Tenancy Deposit" DApp. This distributed app runs on the Etherereum blockchain network and holds a tenancy deposit as a Solidity smart contract.

# Description
Tenancy Deposit DApp keeps a tenant's deposit in an account separate of landlord's one during the renting period and returns it after the tenancy contract terminates.
In case of a dispute between the two parties over the size of the deduction the landlord claims, an arbiter resolves it.

## Landlord
A landlord could:
* create a new tenancy contract
* submit a deduction claim
* withdraw a deduction, which is either approved by the tenant or ruled by the arbiter in favour of the landlord after resolving a dispute

## Tenant
A tenant could:
* sign a tenancy contract thus paying the deposit amount
* submit a deduction claim (in order to agree with or object to landlord's deduction claim
* withdraw the paid deposit or eventually (deposit - deduction), which deduction is either agreed with the landlord or the arbiter resolves a dispute in favour of the landlord and rules given deduction amount

## Arbiter
An arbiter could:
* rule a deduction amount in favour of the landlord in case of a dispute</li>

# Architecture
Please find more about application's architecture at its [Architecture Page](Architecture.md).

# Repositories:
* [Tenancy Deposit Solidity](https://github.com/nvasilev/tenancy-deposit-sol)
* [Tenancy Deposit Client](https://github.com/nvasilev/tenancy-deposit-client)
* Tenancy Deposit Server Side
* Tenancy Deposit IPFS
* Tenancy Deposit Oraclize

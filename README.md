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

# Delivery Plan
## Stage 1: Contract & Contract Tests & UI (MVP)
1. Develop Solidity Contract [`DONE`](https://github.com/nvasilev/tenancy-deposit-sol/blob/master/contracts/TenancyDeposit.sol)
2. Develop Truffle Tests for Solidity Contract [`DONE`](https://github.com/nvasilev/tenancy-deposit-sol/blob/master/test/TestTenancyDeposit.js)
3. Develop "Standalone" UI `IN PROGRESS`
## Stage 2: Distributed Media Support
4. Develop Storing Image(s) and Data for Rental Property to IPFS `PENDING`
## Stage 3: Distributed Media Support
5 Wallet JSON Stored to a Remote Client-Owned Storage (Storj/Dropbox)
## Stage 4: Time-based Oracles
6. Develop Time-based Contract Termination (Oraclize) `PENDING`
## Stage 5: Security (Server Authentication) and UI Actor Segregation
7. Improve Error Handling `PENDING`
8. Develop Sever Part `PENDING`
9. Integrate Server Part with UI (not "Standalone" anymore) `PENDING`
## Stage 6: Server Integration with IPFS
10. Integrate Server Part with IPFS Storage (step 4) `PENDING`
## Stage 7: Multiple Tenants
11. Introduce Multiple Tenants `PENDING`
## Stage 8: Monthly Rent Payment
12. Introduce Monthly Rent Payment `PENDING`
## Stage 9: Improving UI
13. Rewrite UI Using Contemporary Framework (React/Angular?) `PENDING`

# Future Work
* Storing Image(s) and Data (JSON) for Rental Property to IPFS
* Wallet JSON Stored to a Remote Client-Owned Storage (Storj/Dropbox) 
* Time-based Contract Termination (Oraclize)
* Develop Sever Part (Handling Authentication but Not Keeping (Private) Keys)
* Improve Error Handling
* Integrate Server Part with IPFS Storage (step 4) and UI (not anymore "Standalone")
* Introduce Multiple Tenants
* Introduce Monthly Rent Payment
* Rewrite UI Using Contemporary Framework (React/Angular?)

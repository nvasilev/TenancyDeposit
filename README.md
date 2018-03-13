# TenancyDeposit
Welcome to the "Tenancy Deposit" DApp. This distributed app runs on the Etherereum blockchain network and holds a tenancy deposit as a Solidity smart contract.

You could find the application live on the following URL: [`http://tenancy-deposit-dapp.nvasilev.com`](tenancy-deposit-dapp.nvasilev.com)

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

## High Level Architecture

![Tenancy Deposit DApp Architecture](diagrams/TenancyDepositDApp-Architecture.png?raw=true "Tenancy Deposit DApp Architecture")

## Contract State Machine
![Tenancy Deposit Contract State Machine](diagrams/TenancyDepositDApp-StateMachine.png?raw=true "Tenancy Deposit Contract State Machine")

# Repositories:
* [Tenancy Deposit Solidity](https://github.com/nvasilev/tenancy-deposit-sol)
* [Tenancy Deposit Client](https://github.com/nvasilev/tenancy-deposit-client)
* Tenancy Deposit Server Side
* Tenancy Deposit IPFS
* Tenancy Deposit Oraclize

# Future Work

![Tenancy Deposit DApp Future Architecture](diagrams/TenancyDepositDApp-Future-Architecture.png?raw=true "Tenancy Deposit DApp (Future) Architecture")

* Splash Screen while Waiting on Transaction Execution
* Support for compiling contract on the fly
* Add Error Handling
* Storing Image(s) and Data (JSON) for Rental Property to IPFS
* Wallet JSON Stored to a Remote Client-Owned Storage (Storj/Dropbox) 
* Time-based Contract Termination (Oraclize)
* Develop Sever Part (Handling Authentication but Not Keeping (Private) Keys)
* Improve Error Handling
* Integrate Server Part with IPFS Storage (step 4) and UI (not anymore "Standalone")
* Introduce Multiple Tenants
* Introduce Monthly Rent Payment
* Rewrite UI Using Contemporary Framework (React/Angular?)

# Delivery Plan

## Stage 1: Contract & Contract Tests & UI (MVP)
* Develop Solidity Contract [`DONE`](https://github.com/nvasilev/tenancy-deposit-sol/blob/master/contracts/TenancyDeposit.sol)
* Develop Truffle Tests for Solidity Contract [`DONE`](https://github.com/nvasilev/tenancy-deposit-sol/blob/master/test/TestTenancyDeposit.js)
* Develop "Standalone" UI [`DONE`](https://github.com/nvasilev/tenancy-deposit-client)

## Stage 2: Improve Usability and Flexibility
* Add splash screen `PENDING`
* Add error handling `PENDING`
* Add support for compiling contract on the fly `PENDING`

## Stage 3: Distributed Media Support
* Develop Storing Image(s) and Data for Rental Property to IPFS `PENDING`

## Stage 4: Client-side Wallet Stored to a Remote Storage
* Wallet JSON Stored to a Remote Client-Owned Storage (Storj/Dropbox) `PENDING`

## Stage 5: Time-based Oracles
* Develop Time-based Contract Termination (Oraclize) `PENDING`

## Stage 6: Security (Server Authentication) and UI Actor Segregation
* Improve Error Handling `PENDING`
* Develop Sever Part `PENDING`
* Integrate Server Part with UI (not "Standalone" anymore) `PENDING`

## Stage 7: Server Integration with IPFS
* Integrate Server Part with IPFS Storage (step 4) `PENDING`

## Stage 8: Multiple Tenants
* Introduce Multiple Tenants `PENDING`

## Stage 9: Monthly Rent Payment
* Introduce Monthly Rent Payment `PENDING`

## Stage 10: Improving UI
* Rewrite UI Using Contemporary Framework (React/Angular?) `PENDING`


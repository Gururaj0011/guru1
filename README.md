# PhoneCallSelection 

## Overview

This document provides an overview of the PhoneCallSelection smart contract. This Solidity contract facilitates the selection of a SIM card by a designated caller for making phone calls. Additionally, it keeps track of the number of calls made by the caller to the selected SIM cards.

## Usage

### Contract Deployment

Upon deployment, the contract requires the addresses of sim1 and sim2 to be passed as parameters. The deploying account becomes the caller and is granted the authority to select the SIM card.

### Selecting SIM Card

The selectSim function allows the caller to choose between sim1 and sim2 for making calls. Only the caller can invoke this function, and the selected SIM card must be either 1 or 2.

If sim1 is selected, a revert statement prevents further execution with a message stating "no Recharge for sim one." For sim2, the function continues without any further action.

### Checking Calls

The CallsPerOwner function enables the caller to check the number of calls made to the selected SIM card. The caller can check calls twice (2 times) before encountering a restriction.

## Example

1. Deploy the contract by providing the addresses of sim1 and sim2.
2. The deploying account becomes the caller.
3. The caller can use the selectSim function to choose between sim1 and sim2.
4. The caller can use the CallsPerOwner function to check the number of calls made to the selected SIM card.


## License

This smart contract is open-source and released under the MIT License. Refer to the SPDX-License-Identifier for detailed license information.

## Author 
GURURAJ B M

gururaj48103@gmail.com

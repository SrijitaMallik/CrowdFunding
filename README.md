# CrowdFunding

Introduction:-
This project is a basic implementation of a crowdfunding contract using Solidity. The contract allows users to contribute ether to a project, and the project manager can create requests for funds to be allocated to specific recipients.

Contract:-
The contract is located in the contracts folder and is named CrowdFunding.sol. It has the following functions:
sendEth: allows users to contribute ether to the project
getContractBalance: returns the balance of the contract
refund: allows users to refund their contributions if the project deadline has passed and the target amount has not been reached
createRequests: allows the project manager to create new requests for funds
voteRequest: allows contributors to vote on requests
makePayment: allows the project manager to allocate funds to approved requests

How it Works:-
Users contribute ether to the project using the sendEth function.
The project manager creates requests for funds using the createRequests function.
Contributors can vote on requests using the voteRequest function.
If a request receives majority support, the project manager can allocate funds to the request using the makePayment function.
If the project deadline has passed and the target amount has not been reached, contributors can refund their contributions using the refund function.

Variables:-
The contract has the following public variables:
contributors: a mapping of user addresses to their contribution amounts
manager: the address of the project manager
minimumContribution: the minimum amount of ether required for a contribution
deadline: the deadline for the project
target: the target amount of ether required for the project
raisedAmount: the total amount of ether contributed to the project
noOfContributors: the number of contributors to the project
requests: a mapping of request IDs to Request structures
numRequests: the number of requests created

Structures:-
The contract uses one structure:
Request: represents a request for funds, with fields for the description, recipient, value, completion status, and number of voters.

Security:-
This contract has not been audited and should not be used in production without further testing and review.

Code:-
The contract code is located in the contracts folder and is named CrowdFunding.sol.

# PISP API v2.xx


## Payer Initiated use case
### PISP Transfer
![Sequence Diagram](./docs/PISPTransfer_v2.0/PISPTransfer_v2.0.png)

## Payee Initiated use case
### Payer PISP acceptance of conditions 
When a Payer DFSP receives a request to pay for a Payer and that has their account linked to a PISP provider, the DFSP may choose to use the PISP authorization flow to get authorization from the user for the payment.
![Sequence Diagram](./docs/R2P_PISPPayerAcceptance/R2P_PISPPayerAcceptance.png)

### PISP request to pay
Here the PISP has linked their account with a scope that permits the sending of a request to pay request to their DFSP. The Payee DFSP receives this request, validates, and then initiates a request to pay for payment into their linked account. This sequence diagram build on the previous diagram.
![Sequence Diagram](./docs/PISP_R2P/PISP_R2P.png)


## Account linking
Account linking require three stages of authorizing.
1. Permission to release account information to PISP
1. Permission to link account with defined scope
1. Configuration of the credential to be used to authorize payment.

![Sequence Diagram](./docs/PISPAccountLinking_v2.0/PISPAccountLinking_v2.0.png)


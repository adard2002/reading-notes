# Reading 36 Notes

[Home](README.md)

# Payment Processing

## Credit Card Transaction Process
1. Authorization: In this stage the merchant must object approval for payment from their bank
2. Authentication: In this stage the bank verifies the validity of the customer's credit card using fraud protection tools like AVS, CVV, CVV2, CVC2 and CID
3. Clearing and Settlment: In the clearing stage the transaction is posted to both the cardholder's monthy credit card statement and the merchant's statement and occurs with the settlement stage.

## Credit Card Transaction Participants
- Cardholder: There are two types of cardholders, the transactor and a revolver. A transactor repays the credit card balance in full while the revolver only repays a portino of the balance while the rest accrues interest.
- Merchant: This is the store or vendor you are buying things from. This is the person who accepts the credit card payments and also send card info to and request payment authorization from their bank.
- Acquiring Bank/Merchant's Bank: The aquiring bank is responsible for receiving payment authorization requests from the store and sending them to the bank 
- Acquiring Processor/Service Provider: This is a third-party entity which sometimes an arm of the acquiring bank. The processor gives a service or device that allows the store to accept credit cards and send the details. Then it forwards the payment authorization back to the bank.
- Credit Card Network/Association Member: These operate the networks that process credit card payment like Visa, MasterCard, etc. In the transaction process the credit card network being used will recieve the credit card details from getting the processor. Forwarding the payment authorization request to the bank and sends the response to the processor
- Issuing Bank/Credit Card Issuer: This is the financial  institution that issued the credit card involved in the payment. It recieves the payment request from the credit card network and either approves or declines the payment.
# Aadhaar and payments

_Srikanth Lakshmanan, November 2017_

This article briefly explains the role of Aadhaar on various payment systems and the digital payment services through Aadhaar.

There are three payment systems and integrations built around Aadhaar and run by the NPCI.

1. Aadhaar Payments Bridge system \(APB\) .  Service built to facilitate Direct Benefit Transfer \(DBT\) to consumers like LPG subsidiaries.
2. AePS & BHIM Aadhaar . 12 digit clone of card network with biometric authentication.
3. Aadhaar based Remittance Service \(ABRS\) . Enables funds transfer to a person’s Aadhaar number.

### How does Aadhaar-based mapping and seeding work?

It is important to understand the role of seeding and the NPCI before attempting to understand the payment systems. When a customer seeds their Aadhaar number to a bank account, the customer information on bank’s Core Banking System \(CBS\) is updated. This is analogous to updating your PAN in your bank’s CBS and this alone isn't sufficient for Aadhaar based payments.

Since one Aadhaar number can be linked to multiple bank accounts, it is important to define which account is the primary one for transactions. This is done with the help of the NPCI mapper, which maps each Aadhaar number of a bank identifier. When you link a second account to your Aadhaar number, the mapper is updated with the identifier or IIN of the latest bank account added. This design choice in the mapper has led to problems with with LPG subsidies and Airtel Payments Bank where subsidy transfers have gone to the account which has been seeded the most recently.

### Aadhaar Payments Bridge \(APB\)

The Direct Benefits Transfer scheme uses the Aadhaar Payments Bridge \(APB\) to deliver subsidies from a Government agency to recipients directly. LPG subsidy payments is one of the largest use cases of this system. It must be noted that APB is built on top of NACH, National Automated Clearing House. NACH, which processes large volumes of credit and debit transactions in batches, enables direct payments to be made to any bank account. As recently as Nov 2016, this also allowed subsidies to be delivered even for those without Aadhaar by using account numbers directly.

The Aadhaar Payments Bridge instead uses the Aadhaar number of a person and the linked bank account to make the benefit transfer. This is done using the NPCI mapper, which maps Aadhaar numbers to bank account identifiers.

![](https://lh4.googleusercontent.com/NyqmA2r8Z0MmdV95eCEsDpDS2BgXfOEfZ6mYQsxP0P1rpvC71muGhdwhqrgGb9mL9Bwj7tSD89OeKCg5LbqlmClsLaa3kq6bwIJIKQt8EteNaBPLFYzDeJ3ZG0MWI1p2w9ktocv6)

The flowchart above describes the transaction flow in subsidy delivery.

1. Govt department prepares the subsidy list with amount and presents it to its sponsor bank.
2. The sponsor bank verifies the availability of funds with the department and passes the subsidy list to NPCI
3. NPCI looks up the mapper to identify the destination bank \(based on the IIN of the last seeded bank account in its mapper\) to which the subsidy must get credited.
4. Destination bank looks up its CBS to identify to which account the subsidy should get credited. The transaction confirmations go through the chain NPCI -&gt; Sponsor bank -&gt; Government agency. The destination bank also notifies the customer about the subsidy credit.

### AePS

AePS is a payments network that mimics payment card networks in many aspects. Think of the 12 digit Aadhaar as an alias identifier similar to your 16 digit debit card. With card transactions you authenticate with a PIN if you present the card in person, or CVV and OTP or 2FA for online card transactions. With AePS you authenticate with fingerprint or IRIS biometric authentication for payments made through Aadhaar. Remote and online  payments, when the person is not present, are not supported as of now in AePS.

|  | Card payment | Aadhaar payment |
| :--- | :--- | :--- |
| Customer identifier | 16 digit card number | 12 digit Aadhaar number |
| Authentication present | PIN | Biometric \(FP / Iris\) or OTP |
| Authentication not present | CVV, 2FA | OTP |
| Validity | Limited | Lifetime |
| Revocability | Yes | No |
| Bank identifier | BIN | IIN |
| Merchant acquiring device | PoS, digiPoS | Aadhaar PoS, Desktop / Web based apps |
| QR Acquisition | mVISA, MasterPass | BharatQR \(upcoming\) |
| Mobile Acquisition | Bank issued mobile payments, wallet - merchant | Aadhaar Pay / BHIM Aadhaar family of apps |
| Cash in / Cash out | Banks with ATMs, CDMs, Cash Recyclers | Banking correspondentwith Micro ATM / CSC |

Micro ATMs with banking correspondents \(BC\) were developed as an agent model to deliver last mile banking services to reach the unbanked and underbanked masses in rural India. A BC would carry a Micro ATM with cash, and by transacting with the device using fingerprint, one could perform transactions of limited value like cash deposit and  withdrawal, fund transfer, balance enquiry, and mini statement. Interoperability is built similar to that of cards, where in any Aadhaar linked account of any bank can be transacted on any Micro ATM. There are also plans to add AePS network to the ATMs, so one can transact without a card.

### BHIM Aadhaar

Aadhaar Pay is the merchant payment platform built on top of AePS. A merchant has an Aadhaar Pay app of the acquirer bank \(as opposed to POS machine\) and a customer is expected to key in his or her Aadhaar number and perform a biometric authentication to authorize the transaction. Since several banks were unable to build their own apps, a common Aadhaar Pay app called BHIM Aadhaar was developed by NPCI, following its UPI counterpart BHIM.

It’s not just the concept of payment network that is closely mirrored, it’s also the economic model which mimics card payments. This could be largely because it’s a bank led model and banks have been unable to find a suitable economic model to offset the cost of payments. The cost of payments now also involves the incentives for banking correspondents, besides the infrastructure cost for running payment systems.

Banking correspondents come into the picture when a bank is looking to expand its services but it is too expensive or not feasible to set up a branch in a new location. In these cases, the banks are allowed to authorize third parties to conduct limited transactions on their behalf. The correspondents are employed by the bank and are paid a commission for the services such as enrolment, withdrawal, etc. The business model is unlikely to change unless there are significant investments from the state compensating banks for AePS transactions, or banks face stiff competition from neo-banks \(payment banks, small banks\) and non-banks \(PPIs\).

The high / unsustainable MDR for low value payments was probably making banks averse to OFF-US \(inter bank\) AePS transactions causing high failure rates.

### ABRS — Aadhaar based Remittance Service

In ABRS, a remitter can initiate an IMPS \(Immediate Payment Service\) transaction using the beneficiary’s Aadhaar number, which acts as a financial address & which will be linked to the beneficiary’s account number. ABRS facilitates in simplifying the IMPS payment initiation process as in this service the customer will have to input only Aadhaar number of the beneficiary for initiating an IMPS transaction. A key point to note here is, unlike in IMPS, where one has to be registered to mobile banking and have an MMID to receive a payment through IMPS, Aadhaar alone is sufficient to initiate a IMPS transaction and ABRS uses Aadhaar mapper to find destination bank and credit funds.

## Glossary

**AEBA** — Aadhaar Enabled Bank Account — Bank account seeded with Aadhaar number of the customer in the Core Banking System \(CBS\) of the bank becomes an Aadhaar Enabled Bank Account \(AEBA\).

**AMES** — Aadhaar Mapper enabled Services

**AOVS** — Aadhaar Overdraft Validation Service — A feature of PMJDY, the financial inclusion initiative of the government, is it offers small credit in the form of overdraft facility upto ₹ 5000 PMJDY account holders, with the credit guarantee of future subsidy backed to person through aadhaar. To facilitate this, NPCI offers AOVS, which analyzes subsidy inputs in preceding year to provide banks if an account is overdraft worthy.

**IIN** — Issuer Identification Number — A number to identify the bank / non-bank issuer.

**QSAM** — Query service on Aadhaar mapper — To facilitate the effective implementation of ABRS, a new feature was added to NUUP \(USSD based platform on 99\#\) service. Under this new service, the customer will be able to know, whether his or her Aadhaar number is seeded and linked to any bank account number and if yes, then with which bank and when it was last updated. Dial 9999\# on any mobile to check to which bank an Aadhaar is linked.




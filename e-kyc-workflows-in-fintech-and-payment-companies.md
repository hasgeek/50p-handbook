# e-KYC workflows in FinTech and payment companies

## Introduction

KYC or Know Your Customer is a process followed by businesses selling products and services to customers, agents and merchants. KYC is now commonplace for industries like Banks, Insurance companies and export creditors, as well as companies providing financial services or payment based services and is used for both regulatory requirement as well as market segmentation / targeting customers.

KYC in India became mandatory in 2010, but RBI had put out the norms for KYC much earlier. It was adopted by Banks, Financial Institutions and large companies providing financial services to verify the identity of a customer. This was started to prevent money laundering in the financial sector.

> The objective of KYC/AML/CFT guidelines is to prevent banks/FIs from being used, intentionally or unintentionally, by criminal elements for money laundering or terrorist financing activities. KYC procedures also enable banks/FIs to know/understand their customers and their financial dealings better and manage their risks prudently.

The financial regulator in each country defines the parameters of the KYC verification and the proofs to be collected from merchants or vendors. These can be identify, photo or address proof. Each regulator has a definition of which ID constitutes as a valid proof.

KYC was earlier done physically. This meant, any agency or institution which requires customers to do a KYC will have to appoint agents, who would go around verifying people’s addresses with the proof they provided. It is estimated that the cost of the collection of one document for KYC can run between Rs. 100 and Rs. 250. In fact, even now a few FinTech companies still rely on physically verifying users’ identity. These are usually done by setting up partner merchants and empowering them to become banking correspondents to perform related tasks.

## Types of proofs:

For the purpose of identification and for proof of address, income or identity, you’ll need to posses an “Officially valid document” or OVD which can be a driving license, PAN card issued by the Income Tax Department of India, Voter’s ID card issued by the Election Commission of India, job card issued by NREGA duly signed by an officer of the State Government, letter issued by the Unique Identification Authority of India containing details of name, address and Aadhaar number, or any other document as notified by the Central Government in consultation with the Regulator.

### Identity proof

Many services need a person to prove their identity to reduce the risk of money laundering or fraud. While India does not have a mandated document for proving your identity there are a list of documents which can be used. Currently, India does not have a National Identity Document and hence any document in the list can be used to prove one’s identity.

List here: [https://en.wikipedia.org/wiki/Identity\_documents\_of\_India](https://en.wikipedia.org/wiki/Identity_documents_of_India)

### Address proof

Any official document which can be provided as evidence for address of residence from a government body, bank, or utility company is considered as a proof of address. You can find a list of acceptable documents here: [https://legaldesk.com/general/address-proof-documents](https://legaldesk.com/general/address-proof-documents)

## Types of KYC

The process of KYC varies depending on the application of that KYC. KYC can be of the following types:

### Minimum KYC

This was opened for wallets and other small applications where a customer can open an account in a wallet with only a government approved ID. The KYC has a limit of 1 year and will allow the customer to have a maximum of Rs. 10000 in the account. There are additional restrictions placed on the account such as transfer of funds to another wallet or bank account.

### Full KYC

If the customer has documents to prove their identity, then the merchant or the verifier can perform a Full KYC. This process earlier required a physical verification by the merchant or appointed correspondents, but has now been replaced with Aadhaar based e-KYC. This process involves submitting your Aadhaar number to the merchant, who then initiates a request to UIDAI to verify the details. The validity of the KYC is dependent on the response from UIDAI. This method, unlike the minimum KYC is valid for a few years at least. All accounts which have Minimum KYC right now need to convert to a Full KYC account before the expiry of the minimum KYC.

According to a recent notification by the RBI, holders of non-KYC PPI accounts can use the balance remaining in their accounts, but cannot add or transfer the funds to someone else.

## Paper/Physical KYC

### Central KYC

CKYC or Central KYC is an initiative of the Government of India to centralise the verification of KYC among various entities in the financial sector. This initiative reduces the effort of getting KYC verified for each financial entity. This allows an investor to transact/deal with all entities governed or regulated by the Government of India or a regulator once a KYC is done.

### KRA

A KRA or a KYC Registration Agency is an intermediary providing the service of a central KYC across financial entities. This allows residents to perform a KYC with one of the KRAs registered with SEBI:

* CAMS

* CDSL

* DOTEX

* KARVY

* NSDL

Once the initial KYC is done, the KRA issues a KYC identification number, which can be quoted with financial entities for proving that the KYC process has been completed successfully.

## e-KYC

e-KYC or electronic Know Your Customer is the process of collecting and verifying a customer’s identity, without physically collecting forms. e-KYC is the successor of paper-based KYC.

The goal of e-KYC is to reduce the paperwork required for making investments or transactions. It presents a huge advantage over paper-based KYC systems as it allows KYC through media such as video chat.

Aadhaar based e-KYC is gaining traction right now, where you can identify yourself using your Aadhaar linked biometrics.

\#\#\# What is Authentication?

Authentication is defined as the process or action of proving or showing something to be true, genuine or valid. In computing, authentication is the process of verifying the identity of a user or process.

Authentication is the most important part of access control and it’s important to understand what authentication is and what can be authenticated.

There are two common factors used in authenticating something:

* Something you know such as a password or a PIN

* Something you have such as a smart card, mobile phone or a key generator. For brevity, we will assume that biometrics also falls into something you have. Fingerprints and Iris are reasonably unique and can be used as a factor of authentication.

The need for two factors is important as it prevents two scenarios:

1. Preventing malicious use of your Aadhaar number, which is private information.

2. Preventing misuse of your phone or smart card.

In each of these cases, someone trying to gain malicious access to your details or service would need to have both pieces of information to break into your account. For more in-depth reading on private and secret information, check out the post below:

## Aadhaar Authentication based e-KYC

According to e-Mudra, a certifying authority which provides services for Aadhaar based e-KYC, Aadhaar eKYC is a paperless Know Your Customer \(KYC\) process wherein the identity and the address of the subscriber are verified electronically through Aadhaar authentication.![](/assets/1__qrX9v6hqWKXKc_b8eFM7Q.png)

Source: [https://aadhaarapi.com/](https://aadhaarapi.com/)

There are three types of sAadhaar based e-KYC depending on the application and the level of assurance:

### Biometric

**Method:** Verification of resident’s fingerprints of iris

Biometric verification requires the resident to be physically present. A service provider has to be approved by UIDAI to perform these services. Currently, the adoption of Iris scanning is much lower compared to fingerprints. This method is considered the highest assurance among the three types as it requires a resident’s fingerprints or iris, which cannot be duplicated easily and the Aadhaar number.

### Demographic

**Method:** Verification of resident’s demographic data

Demographic data consists of a resident’s details such as name, address, gender or date of birth. A service provider who is collecting data about the resident can verify that the details provided matches the details verified by the resident’s Aadhaar number.

## OTP

**Method:** One Time Password \(OTP\) received on resident’s mobile number

Service providers are also allowed to verify a user’s identity by triggering a verification with Aadhaar OTP. This involves a One Time Password sent to the resident’s registered mobile number, which has to be entered in the application doing the verification or with the merchant who’s requesting it.

## Authentication/KYC User Agency

Entities that aim to do eKYC, need to use services of KUA \(KYC User agency\) or can get a KUA license and operate one themselves. KUA is a licensed entity having access to UIDAI CIDR through KSA \(KYC service agency, which has firewalled access to CIDR\) to retrieve demographic information from UIDAI after a successful authentication.

ASAs or Authentication User Agency is a service provider who can access the e-KYC through a KSA \(KYC service agency\). These agencies are used by businesses to perform authentication services with Aadhaar e-KYC.

## Tokenization and Virtual ID

The UIDAI earlier in January announced the launch of Virtual Aadhaar IDs. These would be a temporary revocable 16 digit random number issued to a resident, which is mapped to an Aadhaar number. This VID can now be given to service providers when they request for it instead of an Aadhaar number.

This move was taken recently amidst growing concerns of being asked to share one’s Aadhaar number for services. While you can generate a Virtual ID online on UIDAI’s website, it’s usage is currently limited to only an address change. Service providers will need to update their workflows to also accept VID instead of Aadhaar numbers. Service providers are expected to fully roll out VID support by June.

Till 2018, eKYC returned back the UID of the consumer to the requesting entity, thereby making cross-linking of databases possible. After the roll out of VID, the consumer can opt to use VID and even if KYC is performed for “limited KYC” requirement, UID will not be shared to the requesting entity and only a unique token would be sent back along with demographic details.

## Issues with Aadhaar e-KYC:

Aadhaar based e-KYC authentication comes with its own set of issues and limitations:

* Unlike CKYC, where the option exists for business to subscribe to updates, eKYC has to be performed by business periodically to prevent data from becoming stale.

* There is an active Supreme Court hearing on the legality of making Aadhaar based e-KYC services mandatory

* Recently, e-KYC services for a lot of entities have been suspended without reason, causing problems for any FinTech trying to onboard new users

* Less reliable than physical verification. The financial entity has to trust the data supplied by the UIDAI and associated partners. This leads to a greater assumption of risk compared to physical verification by the financial entity.

## Cost implications

Although the introduction of Aadhaar based e-KYC services has reduced the cost significantly for players to perform KYC, these FinTechs will have to pay a service provider per authentication they do. For instance, verification for a PAN number might cost around Rs. 15 whereas it might be much higher for verifying a Driving License, Voter ID card or passport.

According to a report in the TOI, a physical KYC verification and on boarding costs about Rs.100 per person whereas when the same verification is done through e-KYC it costs around Rs. 15 per verification.

## The controversy

Recently, KYC has been in the limelight for different reasons. The most important one of these is the misuse of KYC norms by Telecom companies or NBFCs. RBI in 2015 set up the framework for a category of financial institutions called payment banks. These payment banks are essentially restricted bank accounts setup with simplified KYC norms. RBI then even allowed telecom companies to open payments bank accounts with the KYC completed for mobile connections. After the controversy with Reliance Jio and Airtel last year, the RBI revised these norms, making all KYCs done through mobile connections null and void, requiring millions of users to re-authenticate with their payment bank providers and telecos. This rule seems to apply only for telecos as banks are reusing KYC done for full accounts to open wallet accounts as well.

# Resources

1. \[Aadhaar Dashboard\]\([https://uidai.gov.in/aadhaar\_dashboard/ekyc\_trend.php\](https://uidai.gov.in/aadhaar_dashboard/ekyc_trend.php\)\)

2. \[Application For Digital Signature Certificates, Personal Digital Signature, Digital Certificate Application Form \| e-Mudhra\]\([http://www.e-mudhra.com/\](http://www.e-mudhra.com/\)\)

3. \[Aadhaar Integration \| Aadhaar UIDAI Authentication API \| Aadhaar eKYC App Software \| AadhaarBridge\]\([https://www.aadhaarbridge.com/\](https://www.aadhaarbridge.com/\)\)

4. \[Financial Services Company in India \| Financial Solutions \| Karvy\]\([https://www.karvy.com/\](https://www.karvy.com/\)\)

5. \[RBI toughens KYC norms for payments banks in India\]\([https://yourstory.com/2018/02/rbi-now-toughens-kyc-norms-for-payments-bank-in-india-what-does-it-mean/\](https://yourstory.com/2018/02/rbi-now-toughens-kyc-norms-for-payments-bank-in-india-what-does-it-mean/\)\)

6. \[Know All About Paytm KYC – Paytm Blog\]\([https://blog.paytm.com/few-important-changes-in-paytm-from-1st-march-95b31549d6eb\](https://blog.paytm.com/few-important-changes-in-paytm-from-1st-march-95b31549d6eb\)\)

7. \[UIDAI adds another security level VID for Aadhaar; to roll out by June\]\([https://inc42.com/buzz/uidai-adds-another-security-level-vid-for-aadhaar-sets-june-as-deadline-for-full-rollout/\](https://inc42.com/buzz/uidai-adds-another-security-level-vid-for-aadhaar-sets-june-as-deadline-for-full-rollout/\)\)

# Legend

* KUA: e-KYC User Agencies

* AUA: Authorized User Agencies

* NBFC: Non Banking Financial Company

* UIDAI: Unique Identification Authority of India

* CSC: Customer Service Center

* KYC: Know Your Customer

* AML: Anti Money Laundering

* CFT: Combating the Financing of Terrorism




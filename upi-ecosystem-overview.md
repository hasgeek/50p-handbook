# UPI ecosystem overview

_Srikanth Lakshmanan, November 2017_![](https://lh6.googleusercontent.com/oYlrHc4vWbW8SrrDAaDY4z4RmENHofVRkkZWDDCFShmiFJW9RYUlskvwa9RFao0wiecwrL9p_VPU8rhvq4EpREsieQNmkXvJxP0VKFl4xGqKrK2UwCn2BmsKDfx2zYgGE2SYbEdh)

![](https://lh6.googleusercontent.com/oYlrHc4vWbW8SrrDAaDY4z4RmENHofVRkkZWDDCFShmiFJW9RYUlskvwa9RFao0wiecwrL9p_VPU8rhvq4EpREsieQNmkXvJxP0VKFl4xGqKrK2UwCn2BmsKDfx2zYgGE2SYbEdh)

![](https://lh6.googleusercontent.com/oYlrHc4vWbW8SrrDAaDY4z4RmENHofVRkkZWDDCFShmiFJW9RYUlskvwa9RFao0wiecwrL9p_VPU8rhvq4EpREsieQNmkXvJxP0VKFl4xGqKrK2UwCn2BmsKDfx2zYgGE2SYbEdh)On 18 September 2017, Google Tez became the latest UPI app to be launched. With over 70 UPI apps for the user to choose from, where does each player stand in the ocean? Are the third party apps trumping the bank apps? Let us try and understand different players in UPI ecosystem and how they are categorized and positioned in the market.

## Key entities and responsibilities

### Issuer banks

All banks which join the UPI network as an issuer can enable their customers to use UPI Payments Service Provider \(PSP\) apps and transact through UPI. The bank needs to support IMPS, an instant settlement payment product of NPCI and also assist any disputes arising in transactions. While a lot of banks also have their own PSP infrastructure, it is not mandatory for banks to act as PSP. As interoperability is at core of UPI’s design bank customers customers can download any PSP app and link their accounts to use UPI. Issuers also provide a guarantee deposit to NPCI as security to operate in the network. A total of 55 banks, including payment banks have signed up to be UPI Issuers. It is important to note that wallets are not part of UPI at present, but is likely to be added soon.

### National Payments Corporation of India \(NPCI\)

NPCI is the settlement agency which powers the UPI network riding on top of its own existing instant mobile payment product, IMPS. NPCI provides an SDK to all PSPs on UPI network to enable them to provide a consumer facing application which can be built using the SDK. Aside from running the network, NPCI also runs its own PSP backend, customer facing app.

### Payments Service Provider \(PSP\)

A Payments Service Provider is a user facing entity which provides payment service to its consumers, payment infrastructure support to merchants, online and offline. While this is a broad definition of PSP, it can be broken down further as PSP backend and PSP user facing apps.

### PSP backend

A PSP backend maintains customer information, manages issuing and managing virtual payment addresses \(VPAs\), resolves VPAs to user linked bank account for an incoming payment, maintains history of transactions, logs etc. Currently only banks and approved technology partners of banks are allowed to run their own PSP Backend.

As of now, only banks and approved partners can operate PSP Backend. 40 Banks currently operate their own PSP Backend, which is connected to NPCINet. Three non-banking entities, PhonePe, BHIM, and Tez, operate as technical partners of the banks. In addition to building user facing apps, players operating PSP Backend can also provide business solutions enterprises by means of exposing PSP APIs/SDK.

### Non-bank PSP backend — Banking partner/Sponsor Bank

* **PhonePe :** YesBank is sponsor bank for PhonePe and has a partnership agreement. For merchant transactions, YesBank is considered as VPA issuer and any share of MDR earned goes to YesBank, which might have commercial deal with PhonePe.
* **BHIM:** NPCI runs BHIM backend as a special case PSP backend, wherein NPCI has agreement with all issuing banks and consumer’s bank is considered as VPA issuer, even though common @upi is used VPA and a share of MDR earned goes to each respective bank as NPCI is a non-profit.
* **Tez:** Through a special agreement between Google and 4 PSP eligible banks \(Axis, ICICI, HDFC, SBI\), Tez issues VPAs of these 4 banks through a fair distribution and corresponding banks are considered as VPA issuer share of MDR earned goes to respective bank as per agreed commercial deal.

## Apps

For the consumer, over 60 apps are available to use UPI, by creating/managing VPAs, sending, receiving payments. Although the UPI specification mandates required features for an app to qualify as an UPI app \(ability to pay/collect, transaction history, balance check, linking bank accounts, management of VPA, dispute management, handling intents/QR\), different PSPs, app makers with partnerships with PSPs offer different additional features to users.

### Categories of apps

**Mobile Banking app:** Some banks have an embedded UPI section in their existing mobile banking app. While an existing user of the bank can use his bank login and would see a new section in the app to configure and use UPI, new bank users could just the UPI section alone, using the regular onboarding process. A key feature to note in ICICI iMobile app is that the UPI transactions are authenticated by the bank’s own authentication factor, meaning since the user has already logged in to mobile banking using existing authentication mechanism, the bank isn’t using UPI-PIN like other UPI apps and could potentially use its own preferred auth mechanism. pre-auth for trusted low risk payments, debit card grid auth for high risk payments.

Examples: HDFC Mobile Banking, ICICI iMobile, digibank by DBS

**PSP app:** Most banks have preferred to launch exclusive UPI app to share mostly the same set of features having different UI/UX. All apps consume UPI SDK provided by NPCI and interact with their respective PSP backends. Since many features of the app are common, some banks have preferred to launch the app / backend by branding a white label solution with bank’s branding, while others have invested in building the app completely.

Examples:  
Non-bank PSP apps: BHIM, PhonePe, Tez  
Bank built PSP apps: Standard Chartered, Baroda MPay  
White label solution providers: Infrasofttech, OliveCrypto, FSS Tech, LCode Technologies

**Application Service Provider \(ASP\) app:** Except the three non-bank entities running PSP backends, any other private, non-bank entity can develop a UPI app, as a ASP, having a partnership with bank PSP. All such apps use the bank’s PSP SDK, which contains UPI SDK within itself. Newest UPI platform features may take additional time to come to ASP apps, due to the fact that PSPs have to update their SDK with latest version of UPI SDK and ASP app makers are dependent on PSP SDK for their interaction with UPI.

**ASP payments app:** These are apps by fintech, paytech entities to provide payments solutions to consumers. Some of them might offer extra options to integrate with their own wallet, bill payments, split payments. offers, device integration features like NFC etc.

Examples: Chillr, Citrus Pay, Samsung Pay, Cointab

**ASP integrated app:** These are apps are primarily utility apps operating in their own space, wanting to add payments as an additional layer to improve user experience, tightly integrate UPI payments into their payments flows for native UPI experience. This tight integration means the user need not exit the app to make a UPI payment, can manage VPAs, view transaction history right inside the same app.

Examples: Hike, Truecaller, Jugnoo, Uber, CU — UPI Payment & Chat App

**99\#- USSD gateway:** NPCI, which operates UPI platform, IMPS settlement network, and BHIM PSP, also operates its own USSD gateway targeting feature phones. While all other PSPs can acquire only smartphone users, NPCI-BHIM PSP has integrated its backend with USSD interface, making it possible for a feature phone user to use UPI.

## UPI Merchant Payments Ecosystem

Although the growth of merchant ecosystem and P2M payments in UPI are still low, they are growing steadily, primarily driven through online merchant payments like Flipkart, IRCTC, and Uber. The lack of clarity and low MDR regime for digital POS systems, hasn’t helped penetration of merchant solutions in UPI into the mass market. The merchant solutions channel of UPI is about to get some steam when the BharatQR - UPI integration expands and BharatQR gets an more aggressive push.

Although some bank apps allow linking a merchant’s current account to a VPA, thereby allowing self on-boarding to accept UPI payments, each bank and PSP defines a transaction limit for such VPAs. A merchant has to contact the bank to apply as a merchant, similar to onboarding for card acceptance. In addition to providing a merchant VPA, PSPs also provide apps for offline merchants and an API/SDK for online merchants for processing payments through their web/application.

### UPI for face to face merchant transactions \(F2F P2M\)

**UPI Merchant apps/Digital POS:** Some PSPs offer merchants an app through which a storefront cashier can accept payments, either by generating a dynamic QR code which the customer can scan with their app or by entering amount and VPA of customer to initiate a collect request which customer can accept. These apps create an acceptance infrastructure using the mobile of storefront cashier, suited for small merchants. This category of apps might soon merge with BharatQR and become digital POS apps, if not already.

Examples: BHIM LOTZA MERCHANT APP, HDFC Bank SmartHub App, IDBI UPI POS, ICICI Eazypay, SIB MPOS

**UPI @ PoS:** While merchant apps are best suited for small shops with low volumes, the POS machine is nearly inseparable in modern retail and a few POS products support UPI as an additional payment mode supported. The POS machine generates a QR code which a user can scan to make payment and a unique feature of this solution is it creates paper trail for the transaction which increases trust for both merchant and customer, and solves a pain point of storefront cashiers in reconciling digital payments at the end of the day.

Devices: BonusHub, HDFC DiGiPOS, Innoviti, PineLabs Plutus

### UPI for face to screen/remote merchant transaction \(F2S P2M\)

**UPI PSP Merchant SDK:** E-commerce sites, online payment processors, and large enterprises have different, complex payment needs and integration of UPI flows for business need. PSP backends can provide access to these systems through an API or SDK to facilitate custom integration of UPI into merchants’ existing enterprise billing systems to offer their customers better payment experience. Facility to send and monitor collect requests, custom apps, and MIS reporting are some features of merchant solutions offered by a PSP’s SDK.

Players: AxisBank, HSBC, ICICI, PhonePe, Standard Chartered, Tez, YesBank

**Payment processors:** Payment processors integrate several payment channels to enable multi-mode online payments from users. Multiple payment processors have integrated UPI as a payment option and most of them provide the feature as a seamless upgrade without requiring developers using payment processors to change their integration layer. Payment processors typically use the Merchant PSP SDK to complete the transaction. In order to receive a payment through UPI from a customer, an online merchant, app, or payment processor has 2 options.

1. Send and monitor collect request. Ask customer for VPA and send a collect request with amount specified which customer can approve in their UPI app after authorizing using UPI PIN.
2. Subscribe to payment transactions. Send a UPI deeplink to raise an intent and provide details of the transaction in the form of QR code along with a transaction ID, which can be monitored when the customer performs successful payment for the transaction.

Players : CCAvenue, Instamojo, PayU, RazorPay

### On Google Tez’s UPI Bets

As one can see, the ecosystem is wide open and competition is just getting started. Google Tez is latest entrant to operate a PSP backend aside from banks. It gives BHIM and PhonePe tough competition. On the customer applications side, ‘ok’ prefixes on the VPAs of Tez indicate that Google might be eyeing voice mode transactions and could reach across urban and rural markets to emerge as a leader. Banking on huge treasure troves of data and individual preferences, Google also has a significant advantage in offering businesses an edge through its merchant solution. On the other hand, UPI space will increasingly become more crowded and have stronger players when wallets and payment banks, including Paytm join the network and we see rapid changes in the market shares and market segments of each player.


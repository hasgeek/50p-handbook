# **UPI - BharatQR integration**

_Srikanth Lakshmanan, November 2017_

## UPI

Unified Payments Interface is the network powering the UPI/BHIM family of payment apps which let consumers make and receive payments. It has its own QR code specifications. Most UPI apps let users generate a QR code for their VPA and since the specification is open, users can create QR codes following the scheme and use it for receiving payments.

### UPI QR Code Linking Specifications

It’s a URI scheme, which when scanned on a phone can raise an intent to open UPI apps installed on the phone.

* Caters to both P2P as well as P2M transactions with some fields like txnid that are specific for merchant transactions.
* Interoperable across all UPI applications.
* Pre-populates the transaction values, presents to users to directly authorise the transaction without having to enter values. In case of static QR codes, amount needs to be manually entered. Authorization is through UPI PIN.
* Since UPI itself is linked to bank accounts only, option of paying with credit card doesn't arise.
* UPI is a single payment system and flows through a single payment network, hence data is available at NPCI and is published.
* When scanned, UPI QR contains series of values to identify payee and transaction specific metadata:
  `upi://pay?pa=zeeshan@npci&pn=Zeeshan%Khan&mc=0000&tid=cxnkjcnkjdfdvjndkjfvn&tr=4894398cndhcd23&tn=Pay%to%rohit%stores&am=1010&cu=INR&refUrl=https://rohit.com/orderid=9298yw 89e8973e87389e78923ue892`

## BharatQR

The BahratQR code specifications were created jointly by VISA, MasterCard and Rupay to enable digital payments for small merchants without the need for having a POS machine. A consumer having a BharatQR enabled mobile banking app linked to debit or credit cards can scan the merchant’s QR code and complete the transaction. The merchant can choose to generate a static QR code for display in the store and even generate QR codes dynamically for each transaction. When static codes are used, the customer will have to enter the payment amount, while for dynamic codes, the amount and the merchant information is embedded in the QR code itself. The acquirer bank of the merchant allocates different merchant codes for each of the card networks and the transaction goes through depending on the customer’s card network.

* It’s a tag length, value-based string encoding the merchant identifiers which when scanned inside a mobile banking app with BharatQR support can pre-populate transaction values.
* Caters only to P2M transactions, effectively creating a digital, asset-light POS
* Pre-populates the transaction values and presents to users to directly authorize the transaction without having to enter values. In case of static QR codes, amount needs to be manually entered. Authorization may or may not have additional PIN entry, since the app itself is open only after PIN or password.
* Use of credit card permitted, if the support exists in payment app.
* BharatQR is an assortment of payment networks and transactions flow through multiple card networks \(Visa,Mastercard,Rupay\), and other payment networks \(UPI and AePS soon\), data on its usage is hence available at different networks, which are not published by respective owners.
* When scanned, BharatQR looks like `000201010212021644038478002027060415522024078002027061661000307800202700822CITI0100000CITIHDF111152044814530335654071239.005802IN5905ACTTV6006MUMBAI610640005362180514JVH1564533597563041D01`

The text above in italics represent the tag identifiers, and text in bold represent the tag values containing merchant payment identifiers across payment networks, transaction metadata, and merchant information.

### The need for integration

Aside from the notion of “single QR” format, the real reason behind the integration move seems to leverage on other platform’s benefits. The UPI, even after 20 million downloads and growing transaction volumes, is still predominantly P2P, online, app based merchant payments and is hardly seen or accepted in brick and mortar stores even at places where other digital modes are accepted.

BharatQR on the other hand, which inherits the mVISA merchant base, offers incentives to acquiring banks which are more used to traditional modes of merchant acquisition. It rallies behind established existing settlement systems which are used for POS machines as against sometimes troubling IMPS \(Oh where is the data, lets cover it later\) settlement infrastructure. But the downside is, even after a dozen banks updated their apps to integrate BharatQR, consumers do not use it much, compared to popular UPI apps like BHIM and PhonePe which have strong brand recall.

### Integration & Impact

As per a recent NPCI circular, all BharatQR stickers and QR Codes generated after 15 September 2017 must have UPI VPA embedded. All UPI apps must support scanning BharatQR codes and auto populating the transaction similar to a UPI QR code and the transaction would be performed as UPI transaction.

A newer BharatQR deployed might contain UPI handle like this:

`000201010212021644038478002027060415522024078002027061661000307800202700822CITI0100000CITIHDF11110985alphanumeric-merchant-vpa@acquirerbankpsp52044814530335654071239.005802IN5905ACTTV6006MUMBAI610640005362180514JVH1564533597563041D01`

The integration will provide consumers more opportunities to pay using their UPI apps. We may see fewer stickers at shops, as wallets would be soon part of UPI and merchants might be dealing with fewer systems than before, without losing out on the user base.

For acquiring banks, this could drive some volume into their UPI infrastructure and could make them remain invested in UPI, even though their apps might not have been a hit. There was also a talk of integrating Aadhaar Pay into BharatQR a while back. By placing \(almost\) all payment systems into a single QR code, it gives the ultimate choice to consumers to use their preferred payment mode or app.

We are probably going to be surrounded by QR codes sometime soon. Beyond app discovery and installs, browsing pages, and making payments, there will soon be authorised instructions through QR codes as well. UPI e-Mandates has a QR code structure, which can launch the mandate creation screen with pre-populated the values for the standing instructions. Filling forms or calling up your credit card’s customer care to convert purchases to EMI may soon be a thing of past when one can scan a QR code and get a notification on an app to create a SI.


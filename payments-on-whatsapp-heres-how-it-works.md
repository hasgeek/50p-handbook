# Payments on WhatsApp? Here’s how it works.

WhatsApp is among the latest apps to start supporting peer to peer payments using the UPI framework. There has been quite the [controversy surrounding this release](https://www.medianama.com/2018/02/223-paytm-vs-whatsapp-on-upi/) on the features implemented and the NPCI has clarified that the [app will follow all the guidelines](https://www.medianama.com/2018/02/223-npci-statement-calls-whatsapp-payments-launch-a-beta/) set for UPI when the feature rolls out completely.

One of the earliest announcements about this feature was a report by The Ken. You can read more here: [https://the-ken.com/story/whatsapp-upi-payments/](https://the-ken.com/story/whatsapp-upi-payments/)

### Peer to peer payments

When UPI was launched, it was met with a lot of cheer by the apps and services which had struggled to find an easy way to enable payments within the app. One had to use a wallet, escrow service, or a third party service to enable such payments.

There are several problems which UPI aimed at solving with peer to peer payments:

#### **User registration**

Users must be registered with the same bank or service such as IMPS or NEFT. IMPS and NEFT required a login and verification for each transaction and it is very difficult to convince users to store their banking credentials on an app which is not their first party banking app. Chillr was one of the earliest apps to attempt to solve this, by partnering with HDFC bank, making intra-bank payments possible through a third party app. This was not without its own set of flaws. Other bank users had to go through a lengthy process to register their accounts on the app and often, the speed and convenience of making payments was dependent on the backend of IMPS. If you had to make a payment to someone who was not on the platform, you’d need their bank credentials — Account number, IFSC code and phone number or get them to register themselves on the app. This workflow was with a lot of friction, but made peer to peer payments a little easier.

#### Walled garden

A wallet service such as Paytm or FreeCharge required the user to add money to their wallet by using a credit or debit card or bank account. This also meant that users had to keep the money on the wallet platform and make payments with the wallet. This causes significant issues of trust in the wallet apps, since they even charged to withdraw the funds into a bank account.

A’s bank account -&gt; A’s Wallet -&gt; B’s wallet -&gt; B’s Bank.

Using a wallet service also brings forth issues around interoperability. Wallets end up creating a walled garden within which money could be transferred or spent. While not a lot of merchants were allowing payments through wallets, it also meant that a Paytm user could only transfer to another Paytm user. Transfer of money between wallets was not possible. If you had to transfer money back from a wallet to a bank account, the wallet providers would charge a small transaction fee for the transfer. Wallets did counter this by offering users incentives through discounts and cash back, but it was not enough.

#### Old banking infrastructure

The RTGS and NEFT infrastructure were never meant to handle large volumes of small ticket transactions, since there were not too many avenues to make such transactions. Banks charged a small fee on every transaction, which was fixed and it cost the banks significantly if people were making smaller, but more frequent transactions. Transactions through these platforms were slow and confirmations were not delivered instantly. Since the money was routed from one bank directly to another, there were question on liability in case of a failed transaction. IMPS was launched by the NPCI to solve this problem. When Chillr launched initially partnering with HDFC bank, there was a transaction fee of about Rs. 3.5 plus additional service charge. The transfers were capped at Rs. 5,000 per transfer and one could do 10 transactions per day. Even now, banks sometimes charge a transaction fee as high as Rs. 5.90 per transaction when transacting with UPI.

While HDFC users could send and receive money, other bank users had to register on the app and update the bank details, only to discover that their bank did not support outbound transactions. The apps facilitating the transfers also required RBI approval, thus making innovation stunted.

#### Interoperability

While Chillr and first party banking applications serviced the need of those who wanted to transfer money, they did not try to integrate with apps which people were already using — social media, e-commerce and this meant having to convince the users to download the app and use it regularly. This shot up the price of customer acquisition and made it a very expensive business.

With the launch of UPI, it was easy for banks to come on board since the service offered easy integration and had the backing of the NPCI \(National Payments Corporation of India\). While NPCI is not a regulator in the space or a government organisation, NPCI is a conglomerate of a majority of Indian banks. The NPCI backing made it more trustworthy for the banks to integrate with UPI.

Since apps could use the UPI SDK after getting necessary approvals, they could offer peer to peer payments as a feature on the app instead of sending users to a different app. A lot of apps and services such as Truecaller adopted this philosophy with UPI. They already had customers on the platform and it was easy to convince the users to use payments.

Large corporations like Google and Flipkart ventured into the peer-to-peer payments space with the launch of UPI, hoping to get customers to make more transactions. PhonePe and Google Tez are payments apps, but offer little features other than the usual set of features such as bill payments.

Wallet operators and social apps knew they had to jump on this bandwagon or they’d lose customers fast. In fact, Truecaller and Paytm went out of their way to add social features to the apps to draw more users to making payments. Paytm wanted to be the WhatsApp for payments and now offers a lot of features. The messaging features were not great and it was a hard sell for Paytm to convince users to use a wallet app to chat with their friends.

The integration with UPI for WhatsApp was inevitable, given it’s one of the top messaging apps used in India. WhatsApp was looking for a means to expand it’s capabilities and payments on a messaging app is a difficult problem to solve. Services like [Venmo](https://venmo.com/) by Paypal, [Zelle](https://www.zellepay.com/) backed by US banks, [Apple Pay](https://www.apple.com/apple-pay/) and [Google Pay](https://www.blog.google/topics/shopping-payments/say-hello-to-google-pay/) are trying to capture a chunk of the social payments market. Using a messaging service on top of payments offers a huge amount of convenience for users as payments can happen seamlessly. People who traditionally had to go to a banking app to transfer money now send money on chat threads on these apps.

### Beta rollout

UPI for WhatsApp rolled out earlier this month to some users and users have to be prompted for a payment before they can use the feature. It appears alongside the options available in the attachments menu. Users who’ve already registered on UPI can simply link their accounts by verifying their phone numbers. In the beta phase, WhatsApp is only allowing payments to other WhatsApp users who’ve registered for the service. Payments to merchants or non-WhatsApp VPAs have not rolled out completely as of now. Some Android users are reporting the ability to send payments to any VPA on the app, but the feature is not yet supported on the iOS app.

### Auto VPA creation

The regular UPI on-boarding flow requires the user to register a new VPA on the app. This had to be done since the apps partnered with a bank for enabling the features and the VPAs could only be issued by the banks. Some apps like BHIM and Google Tez auto create these VPAs, reducing a step in the registration process for users. This came with its own questions surrounding privacy and anonymity of VPAs, which was one of the important features of UPI. A merchant can simply give out his VPA or create a QR code, which contains no personally identifiable information. Auto-creation of VPAs involve generating the VPA with existing information such as the user’s name or phone number, which raised issues of privacy.

WhatsApp seems to be doing the same thing in its initial beta launch and creates a VPA for you when you sign up. This VPA cannot be changed by the user and we’ll take a look at the VPA scheme later in this article.

### Multi bank backend

WhatsApp has now partnered with ICICI bank to use their backend for transactions. It plans to add support for multiple banks slowly in phases. Having a multi bank backend has several advantages:

* It helps the app balance sudden spurts of requests by spreading the requests across banks.
* It helps the popular apps integrate with BHIM UPI easier, with the choice of partner banks.
* In case of disputes or downtime, the app can easily switch to another backend and continue offering services without interruption.

### VPA scheme

WhatsApp creates a VPA for you and this is `<phone number>.wa.6XY@icici`. The `@icici` will change as WhatsApp begins to add more banks to it’s backend. The `XY` part keeps changing for each VPA and consists of two letters. While the process of auto-creating VPAs certainly makes it easier for users to start making payments, it does not allow someone to create a private VPA, without letting out their phone number.

### Charges, fees and limits

With UPI, peer-to-peer transactions are not chargeable currently, though this may change soon. Traditionally, if there is a payment being made from a customer to a merchant, the merchant is charged a small fee for the transaction. We might see a similar situation with WhatsApp payments as well, where merchants would be able to use the API access to request for payments or have a QR code scanned. These transactions would cost a small fee for the merchant but not the customer.

### Conclusion

Enabling payments on messaging applications opens up a lot of possibilities for users and businesses alike. WhatsApp has already launched its enterprise suite of offerings and companies like ClearTrip and Bookmyshow are already taking advantage of this to send tickets to users via WhatsApp. As and when WhatsApp opens up APIs to request payments, brands will be able to provide the full shopping experience on the same chat thread. These as are effective than using other apps since the whole transaction can be completed without ever leaving the app.

Small businesses can offer a more interactive shopping experience on phone and it becomes easier for services which require recurring billing to send a payment requests on a schedule. Amazon has already added UPI support in India, making it easier to make payments without using a card or net banking.

It is now more than easy to pay your friends back for a meal out or settle IoUs instantly. Bill splitting currently hasn’t been well done, since a large portion of these groups are on messaging applications, whereas the process of splitting bills and settling shares are on another app, which leads to a broken experience.

WhatsApp will slowly roll out support for scanning BharatQR codes and make payments to merchants without having their phone number. This makes WhatsApp very useful on basic smartphones where storage space is a luxury. Users can make payments and stay in touch with a single app instead of downloading apps which have features they don’t need.


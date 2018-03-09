# Thoughts on PayTech business models in India

Sri_ikanth Lakshmanan, February 2018_

Payments Banks were setup as a result of the recommendations of the Nachiket Mor committee on financial inclusion in January 2014. The committee recommended the introduction of specialised banks or payments banks to cater to lower income groups and small businesses. This was an important move to ensure that every Indian resident would have a bank account.

With multiple companies partnering with banks to launch their payments banks, it is important to take a look at what drives the players, impact of commodification of payments, how regulatory landscape impacts business models of Payments Banks and more. While payments banks are more enthusiastic in embracing new technology, there are still some restrictions in India for payments banks:

* Deposits by customers are restricted to Rs. 1 lakh per customer and maybe increased further.

* Payments banks cannot issue loans or credit cards.

* Payments banks have a minimum capital requirement of Rs. 100 crore.

# Bank led payments model

Demonetisation and the subsequent push for digital payments from the government created lot of ripple effects and many, including banks and payment industry players, themselves are unsure of which way the digital push would travel.

Consider the following things:

* [Watal Committee Report](http://watalreport.cashlessconsumer.in/recommendations.html) weighing in favor of a regulatory board inside RBI as against an independent payment regulator.

* [Master directions on PPI](https://rbi.org.in/scripts/BS_ViewMasDirections.aspx?id=11142) \(aka KYC hell for PPI\)

* Interoperability for PPIs envisioned through bank owned settlement network \(NPCI\) payment platform \(UPI\)

* [Bharat QR — UPI](https://blog.50p.in/explaining-upi-bharat-qr-integration-e6f092651ea1) convergence and indirect push towards making it ubiquitous acceptance platform, eventually killing non bank operated acceptance platforms / effectively reducing Prepaid Instruments to Prepaid Issuers, stripping off their ability to run acceptance side business.

* Government subsidizing cost of payments / MDR to small ticket size transactions upto ₹2000 through debit cards / UPI / Aadhaar to banks.

* Global big tech \(Google, Whatsapp, Samsung, Amazon\) had to partner with banks to offer payment products.

All of these suggest, that the government/RBI/at very least certain interest groups wants the entire payments sector to be led by banks and non bank players, be it NBFCs, Fintechs, or global giants have to piggyback banks for operating in the sector.

Although the below graphic shows models around Mobile money across markets, India is bank led when it comes to payments in general, not just mobile \(including agent banking / payments, merchant payments, ATM operations\)

![](/assets/image_preview.png)

Source: GSMA, [Mobile Money Regulation](https://www.itu.int/en/ITU-D/Regional-Presence/ArabStates/Documents/events/2016/DFI/Pre/GSMA_ ITU_Arab States_25 August 2016_BM.pdf)

# Payment infrastructure access & Inter-operability

National Payments Corporation of India \(NPCI\) is a not for profit, private company owned jointly by banks in India operating various retail payment platforms and offers settlement infrastructure for inter bank transactions through various modes.

While traditionally NPCI served the needs of banks and made settlements efficient for banks \(NFS for ATM operations, CTS for cheques\), it entered the terrain of consumer facing products with IMPS and subsequently with Aadhaar subsidy delivery through Aadhaar Payments Bridge \(APB\), Aadhaar enabled Payment Systems \(AePS\) and most recently UPI and BBPS. NPCI is defacto a settlement agency monopoly in India. It is tough to define the role of NPCI, Arundhati Ramanathan puts it better in [The Ken piece](https://the-ken.com/story/npci-god-many-things/) on NPCI,

> Depending on the time and context, NPCI is a competitor. It is a platform. It is a regulator. It is an industry association. It is a profitable non-profit. It is a rule maker. It is a judge. It is a bystander.

UPI was launched as a single inter-operable platform for payments and there have been instances where the actual regulator, RBI, has cited the use of [UPI for inter-operability](http://www.livemint.com/Industry/lOITgGgnJLidZJU5m0IMbP/Interoperable-mobile-wallets-in-six-months-RBI.html) post full KYC \(defacto Aadhaar eKYC\) by wallets. There is also growing perception of UPI being an interoperability standard, while in reality it is a means to an end in achieving interoperability through a centralised platform. Although FinTechs, global big techs have joined UPI, they are still under a bank led model, requiring a partnership with banks to join the platform. Although in some cases, physical access to settlement infrastructure is made available to tech players, it is still a regulated access. So, being a bank is important at some level and gives advantages for entities with serious ambitions on payments, as some core banking infrastructure access is available only to banks, while its good to be in partnership while testing waters, having a license will mean savings on rent paid for partnerships and a “right” into the bank club.

# Bank license, hierarchy, access

Obtaining a bank license in India is a **big deal**. RBI, the regulator for banks is conservative on granting licenses for fear of failures, also has a conflict of interest since govt owns few scheduled commercial banks as public sector undertaking \(PSUs\). [Nachiket Mor committee on Comprehensive Financial Services](https://en.wikipedia.org/wiki/Committee_on_Comprehensive_Financial_Services_for_Small_Businesses_and_Low_Income_Households) for Small Businesses and Low Income Households led to concept of segmented licenses to include small finance banks and payments bank recognized and subsequently licenses issued. The bank license from RBI will mean they can rightfully claim the access to settlement infrastructure and not be at mercy of large banks. But India is a hierarchical society, where does Payments Bank sit amidst, PSU Scheduled Commercial Banks, Private SCBs, MNC SCBs, Cooperative banks \(Urban, District\), Regional Rural Banks of varying sizes?

# Payments Banks

Of the 11 licensees who got the **in-principle** approval from RBI, 3 \(Cholamandalam Distribution Services, Sun Pharma, Tech Mahindra\) have already surrendered licenses.

* Digital / Mobile first Payment Banks — [PayTM](https://www.paytmbank.com/), [Airtel](https://www.airtel.in/bank), Aditya Birla Nuvo, Jio, Vodafone

* Financial Inclusion / Other Payment Banks\* — [FINO](https://www.finobank.com/), [IPPB](https://www.indiapost.gov.in/Financial/Pages/Content/IPPB.aspx), NSDL

Payment Banks come up with a licensing cost. \(100 Crores deposit with RBI\). Does it make sense for a e-wallet company to invest so much, when e-wallets have same infrastructure \(UPI\) access post KYC when it comes to their existing user base? Is this why people felt there is no money to be made in a world with commoditized payments and high regulatory costs with uncertain returns, hence returned licenses?

Different payment banks have different strategies built around them, be it customer acquisition for payments data, solving e-commerce / payments for retail, selling payment solutions to business, cross selling financial services through financial inclusion, building payment solutions for trade, B2B, wholesale digital payments, hope of going higher in bank hierarchy treating Payments Bank as first step.

# Access to rails, \(quasi\) regulated high entry barrier markets

The payments bank license gives a whole layer of regulatory costs to the entities, starting with KYC to branch requirements. But along with that comes access to payment infrastructure rails, which not only allows them to launch products / platforms of today, but a creative payment bank can innovate and build a platform, use the rail as networks in solving B2B, C2G payments and need not restrict itself to current P2P and P2M payments alone. In some sense, access to high entry barrier markets are given as free for holding a banking license. Take the case of bill payments, RBI declared a similar hierarchical structure for any business in bill payments industry and said they have to enroll either as agents, operating units in BBPS, each having its own licensing cost and anyone not doing so must cease and desist from the business of payments. If this is a trend, RBI is bound to put additional licensing requirements for industries / functions that already perform a function of payments, into centralised system requiring licensed access citing interoperability and consumer protection. Fencing more such areas alone can give payment bank licensees a chance to get back their investments including the deposit to RBI.

# Metrics

After a year, since the launch of payment banks in the country, there has hardly been any study about role of payment banks and its impact, except for the report by Bloomberg quint.

[Payments Banks Struggle To Get Deposits Into Bank Accounts](https://www.bloombergquint.com/business/2017/11/20/payments-banks-struggle-to-get-deposits-into-bank-accounts)

[Nearly a year after the first payments bank started operations, this special category of banks has struggled to draw](https://www.bloombergquint.com/business/2017/11/20/payments-banks-struggle-to-get-deposits-into-bank-accounts)

Being an entity, not allowed to lend, or, use deposits in largely high security assets with low returns, the amount of deposits, balance doesn't matter in the context of payments bank. Total money held is useless for digital-only Payments Bank. This is like citing the number of minutes spoken on WhatsApp call. WhatsApp never publishes such information and using millions and billions of transaction value in statistics for payments banks/payments platform will be fooling oneself. What matters is rate of transactions that take place, thereby generating data in the process which can be used to derive value either for commerce or for credit. Some metrics could be

* Number of transactions for digital only PB, data footprint, lending partnerships.
* Number of merchants digitally on boarded for digital only PB.
* Number of banking correspondents, pincodes covered, number of customers, transactions per customer MoM, for Financial inclusion PB.
* Number of business partnerships in selling payments itself as a rails to other sectors there by generating more data, revenue.

Payments is data play for the big tech and data being the fuel to power the AI machines, ones owing oil alone, can run their machines and entities \(governments, corporations, banks, startups alike\) will be like the poorer nations of today that “import” oil and will have high data deficit to sustain.

**Asset Quality**— Data quality will be quality of crude and ability to refine this into valuable data will be key, as at some point market shares will get large numbers, but ability to make profits of that will be dependent on source data and ability to refine them to get insights.

**Technical debt** — Rapidly evolving tech will mean customer experience will keep changing and keeping technical debt in check will be necessity for competing in market. Tech platform owning entities entering into the space will mean, banks and startups can no longer sitback on global technical innovation.

**Credit** — The neo-scoring models are yet to sustain any scrutiny by real world. Market for credit will determine value of data / scores.

**Crypto play** — While crypto is still a niche market in India and there is a void to fill \(privacy friendly \* regulator compliant\) in payments. Can payments see a new generation player upsetting the existing bank led model, much like how it happened in telecom with Jio eating away traditional voice market?

It is still early days for payments banks to be judged, but being a pluralistic society that India is, diverse solutions are needed. The monopolization of bank led payments model and a stackware led centralized payment systems citing interoperability \*\*as shields, while technically interconnect is sufficient. “Open APIs” must be truly open standards and agency monopoly / preference must be ended for a robust competitive market across payment needs, settlement infrastructures for and to invest in solving payments in India.


# Contactless payments

_Abhishek Balaji, December 2017_

Contactless payments use technologies called RFID \(Radio-frequency Identification\) and NFC \(Near Field Communication\) for data transmission which allow for minimal or no contact between the card or user instrument and the terminal. RFID and NFC radios have a longer range than traditional magnetic stripes, making them easier and more convenient to embed in devices. In fact, RFID chips can be made so thin, that they’re used in stickers, posters and advertisements.

When comparing technologies you can use for wireless payments, power usage is an important factor. Every payment system has a terminal and a user instrument. The user instrument is the more portable one and should use less power than the terminal. User instruments can be in the form of a smart device such as a phone, watch or a wearable and even things like key fobs, jewelry, and more.

RFID and NFC chips in the user instruments can draw power from the terminal through electromagnetic induction since the range forces the device to be in close proximity.

There are two modes in which contactless payments can function:

* Passive mode — the communication is between an unpowered device such as a key fob, contactless card or a sticker and a powered terminal. In this case, the terminal creates a field and waits for the other device to come into the proximity field.
* Active mode — the user instrument and the terminal have their own power supplies. A common example for this is when using mobile device for payments using services like Apple Pay, Samsung Pay, Fitbit Pay and others. The typical range to establish communication between the reader and writer is about 4 cm, which also acts as a deterrent for thieves trying to skim your card details. As a security feature, some of the active user instruments start the payments service only when the terminal triggers the NFC chip.

## Types of contactless payments

Payment instruments in India and worldwide can be categorised based on the acceptance networks. Some cards are restricted to certain outlets or retailers, while others can be used across mass transit, retailers and other places.

### Closed loop

These cards are issued by the merchant or a company for use exclusively for goods and services offered by the company or merchant. These cards cannot be used outside the merchant network or for cash withdrawals at ATMs. Closed loop cards are commonly used as prepaid loyalty cards or transit cards, where you can top-up the card and use it for payments exclusively with the merchant.

### Semi-closed loop

Semi closed loop cards are issued by a network of merchants or companies for use within the network. This allows the cards to be more widely accepted by merchants but prevents other transactions at retail locations, including cash withdrawals at ATMs or redemption. These cards can only be used at locations where the merchant is willing to accept the card network and has also signed up with the issuer as a merchant. Examples of semi closed loop cards include those issued by wallet providers like Mobikwik or the Octopus card.

### Semi-open loop

Semi-open loop cards are prepaid instruments which allow all transactions which can normally made using a credit or a debit card, except cash withdrawals. These cards are most commonly issued by loyalty providers, corporate cash management solutions, and some financial services. Examples of semi-open loop cards are those issued by retail chains or shopping malls, which can be used across stores accepting the card network as well as the outlets of the retail chain.

### Open loop

Open loop cards are the regular Visa, Mastercard, Rupay or AMEX cards issued by banks. These cards are the most widely used cards, allowing transactions at most retail locations and online. These cards carry the branding of the card networks they are affiliated to, commonly Visa, Mastercard, Rupay and AMEX.

## How do they work?

NFC or RFID as a communication protocol is not inherently secure, which prevents the devices from transmitting the raw card number and other personally identifiable data. Modern payment methods rely on a technique called as tokenisation, where a token is generated for each transaction. A token is a randomised string which is passed on instead of your card number.

This token is what is passed on the servers of card networks like Visa, Mastercard or Amex where the server verifies the tokenized card number with the data on file. The technology works similar to when you swipe a magnetic stripe card, only that any device which has NFC or RFID built in is able to generate a virtual card. This virtual card is linked to your account in the same way as a regular card and can be used for transactions. This allows users to have a copy of their card on their phones, and the ability to destroy the virtual card in case of theft or misuse.

The flexibility of NFC radios allows the technology to be embedded in a variety of devices and forms while working on very low power. You can find a lot of consumer electronics companies embedding payment solutions in smartwatches, fitness trackers, fashion accessories and even home appliances. The technology is easy to implement and we’re seeing concepts involving cars, refrigerators and other gadgets getting contactless payments. This would allow more flexibility of payments for things like electronic tolls, parking or ordering groceries.

Unlike traditional magnetic stripe or EMV chip based cards, contactless cards don’t have to be handed over to the merchant for swiping on the terminal. Payments are much faster as contactless cards don’t usually require an extra factor of authentication. This allows for quick payments by just tapping the card on the terminal. The lack of second factor also prompts issuing banks to impose a spending limit on each transaction to curb fraudulent transactions. In India, the current limit is Rs. 2000 without a second factor of authentication.

## What is the adoption rate?

Contactless payments haven’t taken off well in India compared to other markets. This can be attributed to a lot of factors. Most banks in India issue POS devices which support only the magnetic stripe and EMV chip cards. The technology for accepting payments through NFC or RFID hasn’t been baked into these POS terminals just yet, so issuers are now relying on incorporating all three protocols in one card. This would allow the card to be used at the full range of terminals used by merchants today. The other issue being, smaller merchants and even retail giants invested in POS devices a few years ago that had only the magnetic stripe technology embedded. The addition of contactless payments does not provide much incentive for these merchants to upgrade, but those who do upgrade to the devices with EMV are getting the benefit of contactless protocol built in.

The benefits of contactless cards begins to show only when you are able to use the technology for seamless payments across mass transit, retail locations, online retailers and even for loyalty and gift cards. Samsung, Apple and Fitbit are betting on this to increase adoption of contactless cards on mobile devices. By scanning and linking the cards to the payment services, virtual cards are created and are stored on the mobile device. This then allows the mobile device to replicate a contactless card, but emitting RFID or NFC signals to the terminal. This level of convenience cannot be replicated by magnetic stripe or EMV based cards that easily, since NFC is very easy and cheap to add to to a phone, but only a few manufacturers like Samsung have incorporated the technology for using these EMV or magnetic stripe cards. In fact, Samsung allows the usage of such cards through Magnetic Secure Transmission or MST on its latest devices. With contactless cards, it is really easy to adapt the technology into mobile devices since most devices have NFC radios built in. Android devices allow third party applications to use the NFC radio, but Apple restricts the usage for anything apart from Apple Pay, its proprietary mobile payments service.

## Are there risks?

As with all credit/debit cards, losing your card can lead to fraudulent transactions. While this was largely mitigated in India through the requirement of a second or even a third factor of authentication in terms of a PIN or an OTP, the new RBI guidelines allow for transactions under Rs. 2000 to be completed without a second factor of authentication. The risks of losing your card are magnified when its use is enabled online with just the information present on the card — card number, CVV and the expiry date. While there aren't too many risks of your card being duplicated in a rogue terminal, the repercussions are reduced, since a contactless card will never have enough information to complete a CNP \(Card Not Present\) transaction. Since details like expiry date and CVV are not stored on the chip, which are required for online transactions, malicious use is prevented.

If you’re planning on using contactless cards on your phone in India, Samsung Pay is the only option right now, with Apple Pay on the horizon. These services add a further layer of security by requiring biometric authentication on your phone as a fingerprint or a face scan. This ensures that even if you lose your device, thieves will not be able to use the phone to make payments without unlocking it first.


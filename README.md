# SeedSigner Guide
This guide demonstrates how to self-custody bitcoin using the SeedSigner. SeedSigner is a project that brings together free and open source code, inexpensive and general-purpose hardware, and a Do-It-Yourself (DIY) approach to taking personal responsibility of your bitcoin. 

![](assets/seedsigner_logo.png)

This guide covers:

- Unboxing the SeedSigner kit
- Downloading & flashing the SeedSigner software
- Testing & assembly
- Generating new wallets
- Securing wallet backup information
- Creating transactions
- Signing transactions
- Multisig

## The Importance of Self-Custody
Before diving into the project, understanding the context for self-custody is a critical aspect of mitigating some of the most pervasive risks involved with Bitcoin, as the saying goes: "Not your keys, not your coins". Trusting third parties like exchanges with your bitcoin introduces several risks that have the potential to leave you vulnerable to theft, seizure, and unrealized capital gains tax. 

Additionally, most custodians, if not all of them, are required to comply with Know-Your-Customer (KYC) regulations that introduce you to even more risks associated with data breaches that leak your Personally Identifiable Information (PII) to the wide open internet. All Bitcoin transactions are public and if your PII is tied to on-chain data then you are left with no privacy against the trusted custodian who knows your identity and your on-chain balances. In the hands of a hacker, that information can put your life at risk. Also, since these custodians prioritize their relationship with law enforcement and will always make decisions that do not have your best interest in mind; in the hands of your government, this information can put your freedoms at risk. 

If you are interested in learning more about catastrophic events involving trusted third parties, check out these resources:

- [Exchange CEO mysteriously "dies" taking $190 million dollars worth of cryptocurrency keys to the grave.](https://decrypt.co/5853/complete-story-quadrigacx-190-million)
- [Cryptocurrency exchange partners with IRS & DEA.](https://decrypt.co/31485/coinbase-license-analytics-irs-dea)
- [Data breach leaks customer information from 30 cryptocurrency companies](https://decrypt.co/95586/hacker-steals-customer-data-circle-blockfi-big-crypto-firms)
- [Argentina introduces "one-off" wealth-tax](https://www.businessinsider.com/one-time-wealth-tax-in-argentina-brought-in-24-billion-2021-5?op=1)

Many of these risks can be mitigated by taking self-custody. The trade off is that you are taking the personal responsibility of securing your bitcoin. You and you alone are responsible for your bitcoin. There are no "1-800" help lines to reverse your transaction and nobody can help you recover a lost or forgotten seed phrase. Luckily there are many tools available to help you achieve safe and private self-custody. 

SeedSigner is one such tool that combines general-purpose, inexpensive hardware with free and open source software to provide you with a DIY signing device so you maintain unrestricted, permissionless access to your bitcoin. Customers of Bitcoin hardware wallet manufactures face certain risks that users should be aware of. There is risk of a supply chain attack where the hardware is intercepted en route and modified in some compromising way prior to final delivery. There is also a risk introduced by exposing personal information to such manufacturers, for example, the [Ledger data breach](https://www.ledger.com/blog/our-communications-about-data-breach) exposed the PII of over one million customers which led to sophisticated phishing attacks and potentially aiding in [physical assault and armed robbery](https://coinidol.com/criminals-steal-cryptocurrency/). There is also the risk of a ["sunset" attack](https://medium.com/cryptoadvance/hardware-wallets-can-be-hacked-but-this-is-fine-a6156bbd199) where the hardware wallet manufacturer could try different nonces until they guess your master private key based on information obtained by watching your transactions on the public blockchain.

One helpful feature of SeedSigner is that the required components are widely available, inexpensive, and general purpose. This means that these parts can be procured in such a way that no indication of using them for Bitcoin is revealed. SeedSigner is sold in a kit from various vendors, so if you purchase the complete kit then it is obvious what the intended use is. However, throughout this guide you will find links to several vendors for the individual components so that you have the resources you need to procure them individually if you prefer.      

## Video Summary
This video demonstrates a high-level overview of the content within this guide. The video is not meant as a replacement for the information in this guide, only as a supplemental visual assistant that demonstrates testing, assembly, generating a seed, entering a passphrase, backing up a seed via QR code, and fire-testing the steel plate.

[![SeedSigner Demo](/assets/VideoThumbnail00.png)](https://media.econoalchemist.com/w/du6mSagqhxYSr5uz8CvnzU "SeedSigner Demo")

## Tradeoffs
No solution is without its tradeoffs, here are a few things to consider with the SeedSigner. A full list of acknowledged criticisms and vulnerabilities is maintained by SeedSigner [here](https://github.com/SeedSigner/independent_custody_guide#alright-but-theres-got-to-be-a-catch-right). To mention a few:

- There is no safety mechanism that verifies the software like found on other hardware wallets. The user is fully responsible for verifying the authenticity of the software used on the SeedSigner. This is explained in detail for both Windows and Linux users in the "Software" section of this guide. Learn how to use the GPG verification tools to mitigate this concern. 
- Saving the private key in a QR code format increases the opportunities that an adversary could get this information. As with any backup information no matter the form, if anyone accesses it they could snap a picture of a list of words or a steel plate or the could just take the backup with them in their pocket. Users benefit from keeping backup information private and secure the way they would handle gold, jewelry, or cash. Having some redundant security in place like a passphrase that is stored separate from the backup information can help mitigate these concerns. Multisig cosigners that are dispersed in different geographic locations can also be beneficial to mitigating a single source of failure.
- Constructing a multisig quorum using the same signing device for all cosigners can introduce a vulnerability if some unforeseen issue arises with that particular signing device. Best practice is to use signing devices from multiple manufacturers to mitigate the risks of a sunset attack and or some security bug that puts your entire multisig balance at risk because you did not diversify the hardware used.  

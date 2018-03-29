## Secure messaging tools beyond Signal

Speaker: [@mshelton](https://twitter.com/mshelton)

- [session description](https://www.ire.org/events-and-training/event/3189/3530/)
- [official slides](https://docs.google.com/presentation/d/1P9-C6TK2GfWZ0CPGkN7YmOeDqNtoktNd6ETueD7EohI/edit#slide=id.p)

> To help ensure the safety of your sources and to empower you to get strong tips, in this session we examine a variety of secure channels that news organizations can offer on confidential tip pages, as well as the relative tradeoffs of these tools.
>
> This session was planned in collaboration with the Freedom of the Press Foundation.

Anonymous tip pages that allow secure messaging! Woo! Basically, if someone's going out of their way to give you information, you should make it as safe as possible for them. Get info, protect sources.

- Who do you want to have your data? Who **cannot** have it?
	- Sources' employers and lawyers?
	- Network operators (ISP, local admin,  the I.T. department)?
	- Shared device/physical access by someone nearby?
	- Malware or remote hackers?
	- Chat providers, like Facebook, Freenode, Matrix, Snapchat, Whatsapp?
	- Government/legal requesters?
	- Competing journalists and news orgs?

"Encryption is pretty effin' great." When done well, encrypting chats gives you more privacy. You can stop network middlemen from reading your messages with sources. And it gives you fidelity: you can know your messages haven't been altered, and you can know if your messages came from the right person.

What does it mean to have a 'private' conversation? Are phone conversations private? No.  Phone conversations convey not just the content of the conversation, but also who's talking, how long, where from. Most chat providers are the same: Facebook, IRC. And most ISPs are pretty much the same as well.

Encrytion hides content.

Metadata is inevitable when you're connecting to the internet. Some apps like Signal don't keep the metadata on their servers. PGP is e2e but isn't designed to protect metadata. Whatsapp keeps some metadata. HTTPS hides the URL you're visiting, but not the domain/subdomain.

When you're having an encrypted conversation, people can tell that you're having an encrypted message.

From a recent survey of popular messaging methods on news organization tip pages:

- Signal
	- devs rigorously avoid retaining metadata. link to the subpoena. They keep account phone number, account creation date, account last active datetime.
	- not designed for anonymity - doesn't stop live metadata surveillance. Don't tell people it's designed for anonymity. Requires a phone number.
	- link to guide about how to set up signal without using your original phone number
	- BuzzFeed's contact page is good.
- WhatsApp
	- Another e2e client, 1 in 7 humans use it, it blends in nicely. User-friendly
	- Turn off cloud synct (iCloud on iphones) because it encourages users to have backups, which means keeping decrypted copies of conversations locally
	- requires phone number
	- owned by facebook, shares a ton of metadata with facebook: link to privacy policy
	- Signal is safer.
- PGP encrypted emails
	- Question from speaker: who has a PGP key? Has sent encrypted email? Received? "Thank you all for coming out here, I know you all survived multiple aneurysms, congratulations on surviving."
	- PGP (Pretty Good Privacy) is a rotocol for encrypting messages anywhere, including email: You're only encrypting the content. You're not encrypting any of the metadata (from, to, subject)
	- mostly used for the least interesting thing possible: email.
	- It's complicated; requires a working knowledge of public key encryption.
	- Voted most likely to give users a headache for over 20 years
	- Doesn't solve metadata problem
- SecureDrop
	- Built to address the metadata problem; built atop Tor. Your ISP doesn't know where you're going within Tor; the site you came from doesn't know where you're coming from. There are special websites that are only accessible within Tor; Tor is not just a proxy or a VPN. SecureDrop runs as one of those onion services.
	- probably the safest option at the moment for having sources contact you.
	- don't use tor at work or anywhere easily tied to you; Tor traffic looks like Tor traffic.
- Physical Mail
	- one-off communication unless the envelope contents have a way for you to reach the person contacting you.
	- USPS scans exterior of physical mail: times link "USPS logging all mail for law enforccement", http://faq.usps.com/?articleId=1449159866675
	- If paranoid:
		- avoid sending from a location easily tied to them
		- avoid using return addresses
	- If talking to prisoners, the mail is expected to be read and possibly censored.
	- Maybe use remailers for physical envelopes.

Don't let sources burn themselves. Warn them ahead of time about metadata. If they need anonymity, use SecureDrop or physical mail; each with their own precautions. For less-sensitive stuff, use the e2e tools.

What tool you want to use depends on who you're talking with. Who they are, who they need anonynimity from.

For anonymizing stuff that has been sent to you, check out witness.org

And if you want to get into the nitty-gritty of why it's hard to make a one-size-fits-all recommendation, read the <abbr title="Electronic Frontier Foundation">EFF</abbr>'s [Secure Mess](https://www.eff.org/deeplinks/2018/03/secure-messaging-more-secure-mess) series publishing this week, about what's necessary for truly secure messaging. What's the safest way to speak to your sources and friends? [It depends](https://source.opennews.org/guides/speaking-securely-sources/).


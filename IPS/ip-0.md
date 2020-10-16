---
squirt: 0
title: IP Purpose and Guidelines
status: Implemented
author: SWAG Finance team
ip: https://ips.swag.finance/IPS/ip-0.html
discussions: https://gov.swag.finance
created: 2020-10-15
---

## What is an IP?

IP stands for SWAG Improvement Proposal, it has been adapted from the SIP (Synthetix Improvement Proposal). The purpose of this process is to ensure changes to SWAG are transparent and well governed. An IP is a design document providing information to the SWAG community about a proposed change to the system. The author is responsible for building consensus within the community and documenting dissenting opinions.

## IP Rationale

We intend IPs to be the primary mechanisms for proposing new features, collecting community input on an issue, and for documenting the design decisions for changes to SWAG. Because they are maintained as text files in a versioned repository, their revision history is the historical record of the feature proposal.

It is highly recommended that a single IP contain a single key proposal or new idea. The more focused the IP, the more successful it is likely to be.

An IP must meet certain minimum criteria. It must be a clear and complete description of the proposed enhancement. The enhancement must represent a net improvement.

## IP Work Flow

Parties involved in the process are the author, the IP editors, and the SWAG community.

:warning: Before you begin, vet your idea, this will save you time. Ask the SWAG community first if an idea is original to avoid wasting time on something that will be rejected based on prior research (searching the Internet does not always do the trick). It also helps to make sure the idea is applicable to the entire community and not just the author. Just because an idea sounds good to the author does not mean it will have the intend effect. The appropriate public forum to gauge interest around your IP is the unofficial SWAG Discord or the unofficial SWAG Telegram.

Your role as the champion is to write the IP using the style and format described below, guide the discussions in the appropriate forums, and build community consensus around the idea. Following is the process that a successful IP will move along:

```
Proposed -> Approved -> Implemented
  ^                     |
  +----> Rejected       +----> Moribund
  |
  +----> Withdrawn
  v
Deferred
```

Each status change is requested by the IP author and reviewed by the IP editors. Use a pull request to update the status. Please include a link to where people should continue discussing your IP. The IP editors will process these requests as per the conditions below.

* **Draft in progress (DRIP)** -- Once the champion has asked the SWAG community whether an idea has any chance of support, they will write a draft IP as a pull request. Consider including an implementation if this will aid people in studying the IP.
* **Proposed** If agreeable, IP editor will assign the IP a number (generally the issue or proposal number related to the IP) and merge your pull request. The IP editor will not unreasonably deny an IP. Proposed IPs will be discussed on governance calls and in Discord. If there is a reasonable level of consensus around the change on the governance call the change will be moved to approved. If the change is contentious a vote among token holders may be held to resolve the issue or approval may be delayed until consensus is reached.
* **Approved** -- This IP has passed community governance and is now being prioritised for development.
* **Implemented** -- This IP has been implemented and deployed to mainnet.
* **Rejected** -- This IP has failed to reach community consensus.
* **Withdrawn** -- This IP has has been withdrawn by the author(s).
* **Deferred** -- This IP is pending another IP/some other change that should be bundled with it together.
* **Moribund** -- This IP has been implemented and is now obsolete and requires no explicit replacement.

## What belongs in a successful IP?

Each IP should have the following parts:

- Preamble - RFC 822 style headers containing metadata about the IP, including the IP number, a short descriptive title (limited to a maximum of 44 characters), and the author details.
- Simple Summary - “If you can’t explain it simply, you don’t understand it well enough.” Provide a simplified and layman-accessible explanation of the IP.
- Abstract - a short (~200 word) description of the technical issue being addressed.
- Motivation (*optional) - The motivation is critical for IPs that want to change SWAG. It should clearly explain why the existing specification is inadequate to address the problem that the IP solves. IP submissions without sufficient motivation may be rejected outright.
- Specification - The technical specification should describe the syntax and semantics of any new feature.
- Rationale - The rationale fleshes out the specification by describing what motivated the design and why particular design decisions were made. It should describe alternate designs that were considered and related work, e.g. how the feature is supported in other languages. The rationale may also provide evidence of consensus within the community, and should discuss important objections or concerns raised during discussion.
- Test Cases - Test cases may be added during the implementation phase but are required before implementation.
- Copyright Waiver - All IPs must be in the public domain. See the bottom of this IPs for an example copyright waiver.

## IP Formats and Templates

IPs should be written in [markdown] format.
Image files should be included in a subdirectory of the `assets` folder for that IP as follows: `assets/ip-X` (for ip **X**). When linking to an image in the IP, use relative links such as `../assets/ip-X/image.png`.

## IP Header Preamble

Each IP must begin with an [RFC 822](https://www.ietf.org/rfc/rfc822.txt) style header preamble, preceded and followed by three hyphens (`---`). This header is also termed ["front matter" by Jekyll](https://jekyllrb.com/docs/front-matter/). The headers must appear in the following order. Headers marked with "*" are optional and are described below. All other headers are required.

` ip:` <IP number> (this is determined by the IP editor)

` title:` <IP title>

` author:` <a list of the author's or authors' name(s) and/or username(s), or name(s) and email(s). Details are below.>

` * discussions:` \<a url pointing to the official discussion thread at gov.swag.finance\>

` status:` < DRIP | PROPOSED | APPROVED | IMPLEMENTED >

` created:` <date created on>

` * updated:` <comma separated list of dates>

` * requires:` <IP number(s)>

` * resolution:` \<a url pointing to the resolution of this IP\>

Headers that permit lists must separate elements with commas.

Headers requiring dates will always do so in the format of ISO 8601 (yyyy-mm-dd).

#### `author` header

The `author` header optionally lists the names, email addresses or usernames of the authors/owners of the IP. Those who prefer anonymity may use a username only, or a first name and a username. The format of the author header value must be:

> Random J. User &lt;address@dom.ain&gt;

or

> Random J. User (@username)

if the email address or GitHub username is included, and

> Random J. User

if the email address is not given.

#### `discussions` header

While an IP is in WIP or Proposed status, a `discussions` header will indicate the URL at [gov.swag.finance](https://gov.swag.finance/) where the IP is being discussed.

#### `created` header

The `created` header records the date that the IP was assigned a number. Both headers should be in yyyy-mm-dd format, e.g. 2001-08-14.

#### `updated` header

The `updated` header records the date(s) when the IP was updated with "substantial" changes. This header is only valid for IPs of Draft and Active status.

#### `requires` header

IPs may have a `requires` header, indicating the IP numbers that this IP depends on.

## Auxiliary Files

IPs may include auxiliary files such as diagrams. Such files must be named IP-XXXX-Y.ext, where “XXXX” is the IP number, “Y” is a serial number (starting at 1), and “ext” is replaced by the actual file extension (e.g. “png”).

## IP Editor Responsibilities

For each new IP that comes in, an editor does the following:

- Read the IP to check if it is ready: sound and complete. The ideas must make technical sense, even if they don't seem likely to get to final status.
- The title should accurately describe the content.
- Check the IP for language (spelling, grammar, sentence structure, etc.), markup (Github flavored Markdown), code style

If the IP isn't ready, the editor will send it back to the author for revision, with specific instructions.

Once the IP is ready for the repository, the IP editor will:

- Assign an IP number (generally the PR number or, if preferred by the author, the Issue # if there was discussion in the Issues section of this repository about this IP)

- Merge the corresponding pull request

- Send a message back to the IP author with the next step.

The IP editors monitor IP changes, and correct any structure, grammar, spelling, or markup mistakes we see.

The editors don't pass judgment on IPs. We merely do the administrative & editorial part.

## History

The IP document was derived heavily from the IP Synthetix Improvement Proposal document in many places text was simply copied and modified. Any comments about the IP document should be directed to the IP editors.

### Bibliography

[SWAG.Finance Discord]: https://discord.gg/SmB9dSh
[SWAG.Finance Telegram]: https://t.me/swagfinance
[pull request]: https://github.com/SWAGFinance/IPS/pulls

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

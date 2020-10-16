# IPs [![Discord](https://img.shields.io/discord/734804446353031319.svg?color=768AD4&label=discord&logo=https%3A%2F%2Fdiscordapp.com%2Fassets%2F8c9701b98ad4372b58f13fd9f65f966e.svg)](https://discord.gg/SmB9dSh) [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-blue.svg)](https://t.me/swagfinance) [![Twitter Follow](https://img.shields.io/twitter/follow/iearnfinance.svg?label=iearnfinance&style=social)](https://twitter.com/swag_finance)

SWAG DAO Improvement Proposals (IPs) describe standards for the SWAG.Finance platform, including core protocol specifications, client APIs, and contract standards.
 
## Contributing

 1. Review [IP-0](IPS/ip-0.md).
 2. Fork the repository by clicking "Fork" in the top right.
 3. Add your IP to your fork of the repository. There is a [template IP here](ip-X.md).
 4. Submit a Pull Request to SWAG.Finance's [IPs repository](https://github.com/SWAGFinance/IPS/).

Your first PR should be a first draft of the final IP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new IP and assign it a number before merging it. Make sure you include a `discussions` header with the URL to a new thread on [gov.swag.finance](https://gov.swag.finance/) where people can discuss the IP as a whole.

If your IP requires images, the image files should be included in a subdirectory of the `assets` folder for that IP as follow: `assets/ip-X` (for ip **X**). When linking to an image in the IP, use relative links such as `../assets/ip-X/image.png`.

When you believe your IP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the IP editors will update the state of your IP to 'Approved'.

## IP Statuses

* **WIP** - a IP that is still being developed.
* **Proposed** - a IP that is ready to be reviewed in a governance call.
* **Approved** - a IP that has been accepted for implementation by the SWAG DAO community.
* **Implemented** - a IP that has been released to mainnet.
* **Rejected** - a IP that has been rejected.
* **Withdrawn** - a IP that has been withdrawn by the author(s).
* **Deferred** - a IP that is pending another IP/some other change that should be bundled with it together.
* **Moribund** - a IP that was implemented but is now obsolete and requires no explicit replacement.

## Validation

IPs must pass some validation tests.  The IP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [yip_validator](https://rubygems.org/gems/yip_validator).

It is possible to run the IP validator locally:
```
gem install yip_validator
yip_validator <INPUT_FILES>
```

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

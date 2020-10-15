# SWIPs [![Discord](https://img.shields.io/discord/734804446353031319.svg?color=768AD4&label=discord&logo=https%3A%2F%2Fdiscordapp.com%2Fassets%2F8c9701b98ad4372b58f13fd9f65f966e.svg)](https://discord.gg/SmB9dSh) [![Telegram](https://img.shields.io/badge/chat-on%20Telegram-blue.svg)](https://t.me/swagfinance) [![Twitter Follow](https://img.shields.io/twitter/follow/iearnfinance.svg?label=iearnfinance&style=social)](https://twitter.com/swag_finance)

SWAG DAO Improvement Proposals (SWIPs) describe standards for the SWAG.Finance platform, including core protocol specifications, client APIs, and contract standards.
 
## Contributing

 1. Review [SWIP-0](SWIPS/swip-0.md).
 2. Fork the repository by clicking "Fork" in the top right.
 3. Add your SWIP to your fork of the repository. There is a [template SWIP here](swip-X.md).
 4. Submit a Pull Request to SWAG.Finance's [SWIPs repository](https://github.com/SWAGFinance/SWIPS/).

Your first PR should be a first draft of the final SWIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new SWIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a new thread on [gov.swag.finance](https://gov.swag.finance/) where people can discuss the SWIP as a whole.

If your SWIP requires images, the image files should be included in a subdirectory of the `assets` folder for that SWIP as follow: `assets/swip-X` (for swip **X**). When linking to an image in the SWIP, use relative links such as `../assets/swip-X/image.png`.

When you believe your SWIP is mature and ready to progress past the WIP phase, you should ask to have your issue added to the next governance call where it can be discussed for inclusion in a future platform upgrade. If the community agrees to include it, the SWIP editors will update the state of your SWIP to 'Approved'.

## SWIP Statuses

* **WIP** - a SWIP that is still being developed.
* **Proposed** - a SWIP that is ready to be reviewed in a governance call.
* **Approved** - a SWIP that has been accepted for implementation by the SWAG DAO community.
* **Implemented** - a SWIP that has been released to mainnet.
* **Rejected** - a SWIP that has been rejected.
* **Withdrawn** - a SWIP that has been withdrawn by the author(s).
* **Deferred** - a SWIP that is pending another SWIP/some other change that should be bundled with it together.
* **Moribund** - a SWIP that was implemented but is now obsolete and requires no explicit replacement.

## Validation

SWIPs must pass some validation tests.  The SWIP repository ensures this by running tests using [html-proofer](https://rubygems.org/gems/html-proofer) and [yip_validator](https://rubygems.org/gems/yip_validator).

It is possible to run the SWIP validator locally:
```
gem install yip_validator
yip_validator <INPUT_FILES>
```

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

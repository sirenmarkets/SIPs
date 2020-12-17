# SIREN Improvement Proposals (SIPs)

SIREN Improvement Proposals (SIPs) describe standards for the SIREN protocol, including core protocol specifications, client APIs, and contract standards.

A browsable version of all current and draft SIPs can be found on [the official SIP site](https://sips.sirenmarkets.com/).

# Contributing

 1. Review [SIP-1](SIPS/sip-1.md).
 2. Fork the repository by clicking "Fork" in the top right.
 3. Start a new thread for your proposal on [gov.sirenmarkets.com](https://gov.sirenmarkets.com)
 4. Add your SIP to your fork of the repository. There is a [template SIP here](sip-template.md). Be sure to link to the discussion thread created in step #3.
 5. Submit a Pull Request to SIREN's [SIPs repository](https://github.com/sirenmarkets/SIPs).

Your first PR should be a first draft of the final SIP. It must meet the formatting criteria enforced by the build (largely, correct metadata in the header). An editor will manually review the first PR for a new SIP and assign it a number before merging it. Make sure you include a `discussions-to` header with the URL to a discussion forum or open GitHub issue where people can discuss the SIP as a whole.

If your SIP requires images, the image files should be included in a subdirectory of the `assets` folder for that SIP as follows: `assets/sip-N` (where **N** is to be replaced with the SIP number). When linking to an image in the SIP, use relative links such as `../assets/sip-1/image.png`.

# SIP Statuses

+ **WIP** - a SIP that is still being developed.
+ **Proposed** - a SIP that is ready to be reviewed in a governance call.
+ **Approved** - a SIP that has been accepted for implementation by the SIREN
  community.
+ **Implemented** - a SIP that has been released to mainnet.
+ **Rejected** - a SIP that has been rejected.

# Preferred Citation Format

The canonical URL for a SIP that has achieved draft status at any point is at https://sips.sirenmarkets.com/. For example, the canonical URL for SIP-1 is https://sips.sirenmarkets.com/SIPS/sip-1.

# Local development

## Prerequisites

1. Open Terminal.

2. Check whether you have Ruby 2.1.0 or higher installed:

```sh
$ ruby --version
```

3. If you don't have Ruby installed, install Ruby 2.1.0 or higher.

4. Install Bundler:

```sh
$ gem install bundler
```

5. Install dependencies:

```sh
$ bundle install
```

## Build your local Jekyll site

1. Bundle assets and start the server:

```sh
$ bundle exec jekyll serve
```

2. Preview your local Jekyll site in your web browser at `http://localhost:4000`.

More information on Jekyll and GitHub pages [here](https://help.github.com/en/enterprise/2.14/user/articles/setting-up-your-github-pages-site-locally-with-jekyll).

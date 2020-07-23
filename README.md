# Open the source :zap:

This document aims to provide a simple rationale for open sourcing and a clear process on how to achieve this in any company. 

For a more in depth guide on building and maintaining open source projects I recommend https://opensource.guide/.

## Why you open source

Your company differentiates itself by offering a core product not by creating the best cloud provisioning tool or the nicest slider implementation (unless that's what you do :smiley:). If you open source, you can get other people to help solve those "infrastructure" challenges.

It's also a great recruitment tool. Developers can look at the code you produce and see how you work, which is the kind of work they might be doing if they join your team.

Developers go the extra mile to improve the quality of a tool they’re sharing with the community.

Some more resources about why you should open source can be found here:

* https://opensource.google.com/docs/why/
* https://opensource.com/life/15/12/why-open-source
* https://github.com/open-source

## When to open source

Generally you don't open source anything that represents core business value.

Everything you open source should be a general purpose tool that can be used by all kinds of people and companies to build all kinds of things.

## Before you open source

* Quality check to make sure you are releasing good, well-tested code - open sourcing is an advert for your team and should be your best quality.
* Ensure that there is no business logic inside the code 
* Ensure there is no mention of your company's name in the code (except copyright statements)
* Ensure there is no sensitive company information inside the code
* Ensure there's a detailed README which documents how to get started and contribute to the project. A Good README example can be found here: https://github.com/wongatech/angular-multimocks/blob/master/README.md
* Truncate any SCM history or use a tool like [BFG](https://rtyley.github.io/bfg-repo-cleaner/) to remove sensitive commit history
* Add a LICENSE file to the root of the repo
    * A common licence is the ISC licence e.g. https://github.com/wongatech/angular-multimocks/blob/master/LICENSE (note company name in file)
    * Set the company name and copyright date
* Get sign-off from your security team
* Get sign-off from your legal team
* Ensure sign-off is in an email for record purposes

## Do you want to be really successful? 

* Add emojis! :sparkles: https://gitmoji.carloscuesta.me/
* Add a [company-styled demo page](http://nabil-boag.github.io/angular-multimocks/)
* Setup a [Travis pipeline](https://travis-ci.com/)
* Add the code to appropriate open source package management like NPM, Bower or RubyGems
* Internal PR: let those who are interested know about the new open source repo
* Build a community: Answer questions on StackOverflow, blog about the project, etc
* Maintain the community: Respond to any feature requests and bugs ASAP

## When merging a pull request

Ensure the following are kept up to date:

* Documentation
* Tests
* Copyright file date field
* Version numbers

## Contacting States

This project contains information on how to automatically and successfully submit the contact forms of state level officials (governors and members of state legislature) who do not provide public email addresses for constituent feedback.

This is what you need to power any system which aims to collect and submit electronic text from US citizens to their elected state level officials.

**Current Status**

We're going through every governor and state legislator who does not have a public email address and codifying their contact form structure into YAML files that follow a simple schema. The `/members` directory already contains a few examples, such as [this description](https://github.com/unitedstates/congress-contact/blob/master/members/B000575.yaml) of how to submit [Roy Blunt's contact form](http://www.blunt.senate.gov/public/index.cfm/contact-form?p=contact-roy).

### Contributing

If you'd like to help:

* [Reply to an open ticket](https://github.com/unitedstates/congress-contact/issues?labels=MoC&page=1&state=open) stating that you are currently working on this issue.
* [Fork this repository](https://github.com/unitedstates/congress-contact/fork).
* [Check out the schema](documentation/schema.md) we're using to represent the steps involved in filling out a member's web form.
* Go visit that representative's website, and fill out a new YAML file describing how to submit the form.
* Save this file in `/members` as `[bioguide].yaml`, where `[bioguide]` is that member's *Bioguide ID*.
* If you don't know their Bioguide ID: you can find it by visiting [bioguide.congress.gov](http://bioguide.congress.gov) and looking at the end of the URL for a given member. For example, Sen. Chiesa's profile at `http://bioguide.congress.gov/scripts/biodisplay.pl?index=C001100` means his Bioguide ID is `C001100`, and so his file would be placed at `/members/C001100.yaml`.
* When you're done, [submit a pull request](https://github.com/unitedstates/congress-contact/compare/) with the new file.

Suggestions on making this process easier are quite welcome.

### FAQ

**So I can drop my contract with `[vendor name here]`??**

This is just data. Even once we have data for everyone, you'll still need to build a system that **integrates** this data. There's nothing here for tracking and storing errors and mistakes, strategies for re-trying, or storing any sort of user data or success statistics.

But what you **won't** have to do is keep up with Congress' constantly shifting websites. That's what this project does.

**Submitting the contact form isn't enough. How do I get other data about members of Congress?**

You can find detailed, reliable data about every current and historical member of Congress at the [unitedstates/congress-legislators](https://github.com/unitedstates/congress-legislators) project.

The data in that project, also stored as YAML, is easily connect-able to this project via each member's Bioguide ID.

### Who's doing this

* [Action Network](http://actionnetwork.org) is in the process of collecting this data.

## Public domain

This project is [dedicated to the public domain](LICENSE). As spelled out in [CONTRIBUTING](CONTRIBUTING.md):

> The project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](http://creativecommons.org/publicdomain/zero/1.0/).

> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
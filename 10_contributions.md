---
layout: default
title: Contributions
nav_order: 10
summary: How to contribute to the Cerberus Protocol.
image: /assets/cerberus_title.png
---

IMPORTANT: This protocol is under development and not yet ready for use.
{: .label .label-red }

Contributions
=============

The cerberus protocol is currently under development and we'll be releasing new sections periodically. This will give us time to gather feedback from bitcoiners who can review our decisions and suggest improvements if necesarry. When it comes to bitcoin security, there's nothing better than peer review!

To provide feedback, let us know in one of the following ways:

* [Bitcoin Design Discord](https://discord.gg/K7aQ5PErht)
* [GitHub](https://github.com/nwoodfine/cerberus)

## Contributor credits
The cerberus protocol has received significant contributions from: 
* [@nwoodfine](https://x.com/nwoodfine)
* [@GorrisR](https://x.com/GorrisR)
* Nicolas Bahmanyar
* [@richardbensberg](https://x.com/richardbensberg)

*Please note that contributions do not necessarily indicate endorsement.*

In addition to the contributors above, we've received invaluable feedback from many friends in the industry that indirectly made its way into cerberus. **Here's a big thanks to those that helped, you know who you are!**

## Upcoming pages you may be able to help with
If you want to help but are short on ideas, here are some pages we're going to gradually get to. 
* Setup ceremony
* Receive a transaction
* Send a transaction
* Hardware wallet recovery
* Hardware wallet replacement
* Personnel changes

## Local development

1. Clone both repositories side by side in the same parent directory:
   ```bash
   git clone https://github.com/nwoodfine/cerberus.git
   git clone https://github.com/nwoodfine/style-the-docs.git
   ```

2. Ensure Ruby 3.2.2 is installed (using a version manager like rbenv or RVM is recommended):
   ```bash
   # Using rbenv
   rbenv install 3.2.2
   rbenv local 3.2.2
   
   # Or using RVM
   rvm install 3.2.2
   rvm use 3.2.2
   ```

3. Navigate to the cerberus directory:
   ```bash
   cd cerberus
   ```

4. Install dependencies:
   ```bash
   bundle install
   ```

5. Run the site locally:
   ```bash
   bundle exec jekyll serve
   ```

6. View the site at: http://localhost:4000/cerberus/

## External theme

This site uses a custom fork of [Just the Docs](https://github.com/just-the-docs/just-the-docs) located at:
https://github.com/nwoodfine/style-the-docs
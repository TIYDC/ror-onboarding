---
title: Computer
layout: default
order: 3
---

# Computer Setup

## Hardware

All students must bring their own MacBook laptop. Your MacBook should have a
minimum of 4 GB of RAM and 128 GB of hard drive space. Those are minimum specs,
but I REALLY recommend getting 8 GB of RAM.

Here are the current
[MacBook Air models](http://www.apple.com/macbook-air/specs.html) and
[MacBook Pro models](http://www.apple.com/macbook-pro/specs-retina/).

Your MacBook MUST be running macOS Sierra which is a free upgrade from the mac AppStore.

Do not go with the new, skinny 12" Retina MacBooks.  Their processor will be too
sluggish in a year or two.

There is no commercial software required for the class.

## Software

### macOS Sierra

You'll need to install macOS Sierra if your Mac didn't have it pre-installed or you haven't upgraded already.

1.  Download the macOS Sierra upgrade from the Apple Store: [download here](https://itunes.apple.com/us/app/macos-sierra/id1127487414?mt=12).
2.  You'll need to sign in to your Mac's 'App Store' with your [Apple ID](https://appleid.apple.com/).
3.  Double-click "Install macOS Sierra" to begin installation.
*WARNING*: The macOS upgrade can take a bit of time to complete and will require a restart. Plan on doing this in the evening or over a lunch break.

### Additional Software

As soon as possible after receiving your Mac, run through the following steps.
If you've done a lot of your own configuration, some of these steps may have to
change.  If you run into ANY PROBLEMS, send me an e-mail at: [{{site.instructor_email}}](mailto:{{ site.instructor_email }})

#### Install Atom

  * Download Atom from [the Atom website](https://atom.io/).
  * Install and run it.
  * Click on the "Atom" option in your menu bar (all the way in the upper-left of your screen) and choose "Install Shell Commands."

**Atom is not the best editor, but it has great defaults, if you are already using an editor stick with it, alternatives, are Sublime Text, SpaceMacs, and MacVim**

#### Install Google Chrome

  * Download Chrome from [the Chrome download page](https://www.google.com/intl/en/chrome/browser/).
  * Install and run it.  This install will work a little differently from Atom, so if you get confused, [read more here](mac_installations.html).

#### Install iTerm2

The terminal is our text-based interface into the computer. It is much more powerful than graphical user interfaces (GUI's) generally and will be more efficient for us in the long run. MacOS comes with a terminal built in, but many people prefer a program called iTerm2.

  1. Download iTerm2 from [the iTerm2 website](https://www.iterm2.com/downloads.html)
  1. Unzip the downloaded file by double-clicking on it.
  1. Open your Applications directory by clicking on the Finder and selecting it from the left sidebar.
  1. Drag the unzipped iTerm application into the Applications folder.

#### Install XCode Command Line Tools

  * Open up iTerm2.  If you're not familiar with opening applications on your Mac, [read this page, especially the last section](mac_installations.html).
  * Go to the [Apple Developer Downloads site](https://developer.apple.com/downloads/).
  * `xcode-select --install`

#### Install Homebrew

  * Open up iTerm2 (or if you've still got it open, keep using it).
  * Run ```ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"```
  * Run `brew doctor`

#### Install rbenv & ruby-build

  * Open up iTerm2 (or if you've still got it open, keep using it).
  * `brew install ruby-build rbenv`
  * `echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile`

#### Install ruby 2.4.0

  * Close and reopen iTerm2.
  * `rbenv install 2.4.0`
  * Go and get some coffee. That last one will take a while.
  * `rbenv global 2.4.0`
  * Close and reopen iTerm2.
  * `gem install pry`
  * Run `which ruby`. If you see a path starting with `/usr/bin/`, get a TA or instructor to help you.

#### Install nodejs

  * In iTerm2
  * `brew install nodejs`

#### Install git

  * In iTerm2
  * `brew install git`
  * `git config --global push.default simple`
  * `git config --global credential.helper osxkeychain`

#### Install Heroku Toolbelt

  * Download the Toolbelt from [this page](https://toolbelt.heroku.com/).
  * Run it and follow the install steps.
  * Open Terminal and run `heroku login`.  Enter your Heroku credentials when asked.

#### Setup SSH key

Create an SSH key (__do not__ give it a password when it asks for one)

  * `ssh-keygen`
  * Press enter at the first prompt to stick with the default file name.
  * Press enter at the second prompt to give it no password.

#### Setup Dock
Add the following applications to your Dock

  * Atom
  * Chrome
  * iTerm2

## Yosemite Upgrade Tweaks

I switched to OS X 10.10 Yosemite a couple weeks after the Beta release. While it's been surprising stable, there are a few things I've had to tweak for development. Compiling a list here.

#### Homebrew was dead [fixed]
I followed this: http://jcvangent.com/fixing-homebrew-os-x-10-10-yosemite

#### Ruby/RVM/Ruby Gems was fishy [fixed..enough]
I think this has something to do with the system update to Ruby 2.0.

I followed the advice here: http://stackoverflow.com/a/9510209/3622553. I forget what the fixed, but it fixed something.

I was using Ruby 2.0 through RVM. It was still acting crazy so I tried http://stackoverflow.com/a/22310466/3622553. That didn't work for me, something went nuts during reinstalation of 2.0. So I just installed Ruby 2.1.0 with RVM and set that to my default.

#### Sass was dead [fixed]
Not sure what the culprit was here, something to do with the Ruby oddness. After doing the above business all seems to be well.

#### Foreman was gone [fixed]
I'm not sure if I just uninstalled this somehow and didn't remember it, but https://github.com/ddollar/foreman was missing. After fixing Homebrew I installed it again with `gem install foreman`

#### Bash Completion is dead [fixed]
I removed anything related to it from my .bash_profile and followed the instructions here http://code-worrier.com/blog/autocomplete-git Working great again.

#### Wireless Mouse Bluetooth was going nuts [fixed]
I would be using the mouse normally and then it would just start sputtering and working all half-assed. Damn near threw it out the window. I deleted the bluetooth plist file like this said: http://www.imore.com/how-fix-mavericks-wi-fi-zapping-bluetooth and that seems to have fixed it.
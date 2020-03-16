- Ignore this section if you're not going to export iOS builds for now

# Fastlane


[Fastlane](https://fastlane.tools/) is a set of tools with the goal of automating all processes related to app development

For now we only use [Match](https://docs.fastlane.tools/actions/match/) which deals with iOS profiles and certificates.

The fastlane/match configuration is already present the in repository you're working on, but before you can use it we have to install some stuff:
Make sure you have ruby/rbenv configuration done correctly
```bash
cd path/to/repo
rbenv install #make sure the ruby version required is installed
gem install bundler -v "$(grep -A 1 "BUNDLED WITH" Gemfile.lock | tail -n 1)" # to install the exact version of bundler we need
bundle # this installs the needed libraries
bundle exec fastlane match development # This is so you can run builds directly to devices from your machine
bundle exec fastlane match adhoc # this is so you can archive and build an adhoc release (to upload to firebase app distribution for example)
```

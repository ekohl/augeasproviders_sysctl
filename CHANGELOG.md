# Changelog

## 2.4.0

- Add Archlinux support (GH #38)
- Use : as separator on FreeBSD (fix #24) (GH #30)
- Do not manage comment when persist is false (fix #29) (GH #31)

## 2.3.1

- Fix puppet requirement to < 7.0.0

## 2.3.0

- Add support for Puppet 6
- Deprecate support for Puppet < 5
- Update supported OSes in metadata.json

## 2.2.1
- Added support for Puppet 5 and OEL

## 2.2.0
- Removed Travis tests for Puppet < 4.7 since that is the most common LTS
  release and Puppet 3 is well out of support
- Added OpenBSD and FreeBSD to the compatibility list
- Added a :persist option for enabling saving to the /etc/sysctl.conf file
- Added the capability to update either the live value *or* the disk value
  independently
- Now use prefetching to get the sysctl values
- Updated self.instances to obtain information about *all* sysctl values which
  provides a more accurate representation of the system when using `puppet
  resource`
- Updated all tests

## 2.1.0
- Added a :silent option for deliberately ignoring failures when applying the
  live sysctl setting.
- Added acceptance tests

## 2.0.2

- Improve Gemfile
- Do not version Gemfile.lock
- Add badges to README
- Munge values to strings
- Add specs for the sysctl type

## 2.0.1

- Convert specs to rspec3 syntax
- Fix metadata.json

## 2.0.0

- First release of split module.

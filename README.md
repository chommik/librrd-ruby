librrd
======

# Description

This gem includes the [RRDtool](http://www.mrtg.org/rrdtool/) Ruby bindings from
the RRDtool sources. It should help people that are unable to use or don't have
some kind of `librrd-ruby` operating system package.

The `extconf.rb` tries to guess the librrd version installed on your system.
If it doesn't work, please try to adjust the `ext/librrd/extconf.rb` file
and submit a pull request or open an issue.

The following systems, RRDtool versions and Ruby versions  have been tested.

* Ubuntu 10.04 LTS (RRDtool 1.3.8)
  * Ruby 1.9.2p0, 1.8.7p302
  * Rubinius 1.1.0, 2.0.0pre
  * ruby-enterpriseedition 1.8.7 2010.02
* Ubuntu 11.04 (RRDtool 1.4.3)
  * Ruby 1.9.2p180, Ruby 1.8.7p334
* CentOS 5.5 (RRDtool 1.2.27)
  * ruby-enterpriseedition 1.8.6 20090610
* OpenBSD 4.8 (RRDtool 1.2.30)
  * Ruby 1.9.2p0, 1.8.7p302
* Mac OS X 10.7.2 (RRDtool 1.4.5, Homebrew)
  * Ruby 1.9.3p0

# Installation

Make sure you have the development package of `librrd` installed.
(like `librrd-dev` on Debian/Ubuntu) Then you can just `gem install`.

    gem install librrd

# Developing

Build the C extension:

    rake build_rrd

Run the tests:

    rake test

# Contribute

Please test the gem on different systems with different RRDtool versions
and report success and/or failure. Open issues and/or submit pull
requests with fixes.

Thank you!

# Links

* Source: http://github.com/bernd/librrd-ruby

# Maintainer

Bernd Ahlers

# Copyright

Since the files have been taken from the [RRDtool](http://www.mrtg.org/rrdtool/)
sources, all files in this project are available under the
[GNU General Public License](http://www.gnu.org/copyleft/gpl.html). See the
COPYING and COPYRIGHT for details.

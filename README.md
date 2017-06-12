Copyright (c) 2011 Float Mobile Learning
http://www.floatlearning.com/
Extension Copyright (c) 2013 Weptun Gmbh
http://www.weptun.de

Extended by Ronan O Ciosoig January 2012

Extended by Patrick Blitz, April 2013

Extended by John Turnipseed and Matthew Nespor, November 2014
http://nanonation.net/

Extended by Nicolas Bachschmidt, October 2015

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Please let us know about any improvements you make to this script!
./floatsign source "iPhone Distribution: Name" -p "path/to/profile" [-d "display name"]  [-e entitlements] [-k keychain] [-b "BundleIdentifier"] outputIpa


Modifed 26th January 2012

new features January 2012:
1. change the app display name

new features April 2013
1. specify the target bundleId on the command line
2. correctly handles entitlements for keychain-enabled resigning

new features November 2014
1. now re-signs embedded iOS frameworks, if present, prior to re-signing the application itself
2. extracts the team-identifier from provisioning profile and uses it to update previous entitlements
3. fixed bug in packaging if -e flag is used
4. renamed 'temp' directory and made it a variable so it can be easily modified
5. various code formatting and logging adjustments

new features October 2015
1. now re-signs nested applications and app extensions, if present, prior to re-signing the application itself
2. enables the -p option to be used more than once
3. ensures the provisioning profile's bundle-identifier matches the app's bundle identifier
4. extracts the entitlements from the provisioning profile
5. copy the entitlements as archived-expanded-entitlements.xcent inside the app bundle (because Xcode does too)


Extended by Henry ( https://github.com/henry42/ ) June 2017

Logging functions

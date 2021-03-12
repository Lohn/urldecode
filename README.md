# urldecode

decode URL data

# Install

Available as a [bpkg](http://www.bpkg.sh/)
```sh
bpkg install [-g] lohn/urldecode
```

# Old README

```
##########################################################################
# Title      :	urldecode - decode URL data
# Author     :	Heiner Steven (heiner.steven@odn.de)
# Date       :	2000-03-15
# Categories :	File Conversion, WWW, CGI
# SCCS-Id.   :	@(#) urldecode	1.4 04/03/03
##########################################################################
# Description
#	Decode data according to
#	    RFC 1738: "Uniform Resource Locators (URL)" and
#	    RFC 1866: "Hypertext Markup Language - 2.0" (HTML)
#	    RFC 2396: "Uniform Resource Identifiers (URI): Generic Syntax"
#
#	This encoding is used i.e. for the MIME type
#	"application/x-www-form-urlencoded"
#
# Notes
#    o	The default behaviour is to decode each line independently of the
#	other, and print the results on an own line. If the line
#	endings are encoded, too (i.e. "%0A" or "%0D%0A"), use the
#	"-l" option to prevent urldecode from adding additional line
#	endings.
#
#    o	Large lines (or binary files) will break many AWK
#    	implementations. If you get the message like
#		awk: record `%3A%0A%23%23%23%23%2...' too long
#	consider using GNU AWK (gawk).
#	If the input line was generated using "urlencode -l", try to
#	omit the "-l" option, if applicable.
#
# See also
#	urlencode
##########################################################################
```
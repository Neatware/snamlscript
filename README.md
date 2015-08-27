# SnamlScript

- A Language of HTML5 Template Generator for Cloud Apps

## 0. New features

v5.1.0
* more readable with multiple parameters for all commands
* support Meteor Blaze binding commands like each, if, with
* support SVG commands

## 1. Introduction

A Cloud App can be a Web, Mobile, IoT, SDN, or Storage Application.

SnamlScript is a commandline language which is similar to Tcl. Block commands and inline commands implemented HTML5, SVG, Meteor Blaze and other internal functions for Cloud Programming. SnamlScript code can generate HTML5 web pages and documents. SnamlScript programs make Cloud Apps more maintainable, modifiable, and reusable with high-level consistence. In addition, SnamlScript is much easier to work along with Cloud Platforms and various JavaScript frameworks such as jQuery, AngularJS, Meteor, .etc. SnamlScript also works for multiple Operating Systems such as Window, Linux, MacOSX, .etc.

Neatware released SnamlScript as Open Source in Apache 2.0 License.

## 2. Source Code

SnamlScript 5.1 implementation was presented in source code snaml5.tcl. pkgIndex.tcl is the file to make snaml5.tcl as a package of tcl.

## 3. Run on Windows

This is the SnamlScript demo with Samples on Windows.

- Download SnamlScript.zip for Windows.
- unzip SnamlScript.zip
- "cd SnamlScript\bin" in command console
- "snamlscript.exe" launch snamlscript
- "cd ..\samples\angularhello" to sample folder
- "source angularhello.sml" to generate angularheoo.sml
- "start angularhello.html" to launch browser
- "notepad angularhello.sml" modify .sml code

## 4. Mac OSX and Linux

Since current SnamlScript was implemented by Tcl which has been pre-installed in most OSX and Linux platforms, you may "source snaml5.tcl" to load SnamlScript and run .sml codes.

## 5. SnamlScript Syntax Highlight

SnamlScript syntax highlight for Atom editor is available on GitHub. Simply type

apm install snamlscript-syntax

you can work SnamlScript with syntax highlight in Atom for Windows, MacOSX and Linux.

## 6. Simple Example

'''
# Use SnamlScript package
package require SnamlScript

# output to a file.
output hello.html

# declare document type as html
__doctype html

# html header
_html "lang='en'"
  _head
    # quote command render a string
    _title; quote Hello; title_
  head_

  _body
    # you can leave space in a line
    __img src='hello.gif' alt='hello'
    quote "Hello World!"
  body_
html_
'''

## 7. Copyrights

Neatware owns the copyrights of SnamlScript.

HTML5, Javascript, CSS are copyrights of one of International Standard Organization.  
Meteor, Angular, Tcl are the copyrights of other third parties in Open Source.

Copyrights (c)2014 Neatware. All rights reserved.

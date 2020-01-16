# Ainur

[![Build Status](https://travis-ci.org/xyproto/ainur.svg?branch=master)](https://travis-ci.org/xyproto/ainur) [![GoDoc](https://godoc.org/github.com/xyproto/ainur?status.svg)](http://godoc.org/github.com/xyproto/ainur) [![License](http://img.shields.io/badge/license-MIT-green.svg?style=flat)](https://raw.githubusercontent.com/xyproto/ainur/master/LICENSE) [![Report Card](https://img.shields.io/badge/go_report-A+-brightgreen.svg?style=flat)](http://goreportcard.com/report/xyproto/ainur)

Go module for figuring out which compiler and compiler version was used for compiling an executable file for Linux (in the ELF format).

### Utilities that uses Ainur

* [elfinfo](https://github.com/xyproto/elfinfo) | [webpage](https://elfinfo.roboticoverlords.org)
* [cdetect](https://github.com/xyproto/cdetect)

### Features and limitations

* Supports detection of compiler name and version if an executable was built with one of these compilers:
  * GCC
  * Clang
  * FPC
  * OCaml
  * Go
  * TCC (compiler name only, TCC does not store the version number in the executables)
  * Rust (for stripped executables, only the compiler name and GCC version used for linking)
  * GHC
* Works even with stripped executables.
* Should work for recent versions of all of the above compilers. Executables produced with old versions of the compilers may need more testing.

### General info

* Version: 1.1.2
* Author: Alexander F. Rødseth &lt;xyproto@archlinux.org&gt;
* License: MIT

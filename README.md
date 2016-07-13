# epanet-dev

This is a collaborative project to develop a new version of the EPANET computational engine for analyzing water distribution systems.

## Introduction

The last major update to EPANET, version 2.0, was made in 2000. Since that time many new advances in water distribution system modeling and suggestions for improving EPANET have been made. This project seeks to develop a new version of the EPANET computational engine and its associated API that includes many of these advances and improvements. It is currently using EPANET 3 as its working title. Written in C++, it employs an object oriented approach that allows the code to be more modular, extensible, and easier to maintain.

EPANET 2 was originally developed by the U.S. Environmental Protection Agency (USEPA) and placed in the public domain. The new version being developed by this project represents an independent effort that is part of the [Open Source EPANET Initiative](http://community.wateranalytics.org/t/announcement-of-an-open-source-epanet-initiative/117) and is neither supported nor endorsed by USEPA.

## Installation

The source code can be compiled to either a stand alone executable or to a shared library whose functions are defined in the header epanet3.h. Any C++ compiler that supports the C++11 language standard can be used.

## API Reference

The EPANET 3 API has a similar flavor to version 2, but all of the functions have been re-named and require that an EPANET project first be created and included as an argument in all function calls. (This makes the API capable of analyzing several projects in parallel in a thread safe manner.) EPANET 3 is able to read EPANET 2 input files but uses a different layout for its binary results file. Thus it will not be compatible with the current EPANET 2 GUI. Details of the API, including the changes and additions made to various computational components of EPANET, can be found in the 'docs' section of this repository (to be added shortly).

## License

The new version of EPANET will be distributed under the MIT license as described in the LICENSE file of this repository.
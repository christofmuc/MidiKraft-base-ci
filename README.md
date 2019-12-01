# Introduction

[![Build status](https://ci.appveyor.com/api/projects/status/52klm4799jyv2op6?svg=true)](https://ci.appveyor.com/project/christofmuc/midikraft-base-ci)

[![Build status](https://ci.appveyor.com/api/projects/status/52klm4799jyv2op6/branch/master?svg=true)](https://ci.appveyor.com/project/christofmuc/midikraft-base-ci/branch/master)


This is only a super-repository for the CI for my utility library [MidiKraft-base](https://github.com/christofmuc/MidiKraft-base.git). Go there for more details on the classes offered. This repository is only to build the library separately by the CI,
as I really want to avoid nested submodules in my projects. 

## Usage

This repository allows us to build the juce-utils library independantly in an easy way. First checkout recursively:

    git clone --recurse-submodules -j8 https://github.com/christofmuc/MidiKraft-base-ci.git
	
Then use CMake to build the makefile for Windows (use other generators as you see fit):

    cmake -S . -B Builds\Windows -G "Visual Studio 15 2017 Win64" 
	
Building with cmake:

    cmake --build Builds\Windows --config=Release

## Licensing

As some substantial work has gone into the development of this and related software, I decided to offer a dual license - AGPL, see the LICENSE.md file for the details, for everybody interested in how this works and willing to spend some time her- or himself on this, and a commercial MIT license available from me on request. Thus I can help the OpenSource community without blocking possible commercial applications.

## Contributing

All pull requests and issues welcome, I will try to get back to you as soon as I can. Due to the dual licensing please be aware that I will need to request transfer of copyright on accepting a PR. 

## About the author

Christof is a lifelong software developer having worked in various industries, and can't stop his programming hobby anyway. 

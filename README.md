# Base Library

## Contents

1. [Motivation](#motivation)
2. [The Goal](#the-goal)
3. [Background](#background)
4. [Description](#description)
3. [Repository Design](#repository-design)
4. [Tests](#Tests)
5. [Support](#Support)
6. [Requirements](#Requirements)
7. [Documents](#Document-List)

## Motivation

This started out as an XTS library, then became something else, a huge crawling repo with too much stuff doing too many things. So it's been broken up into numerous libraries which will break out the elements into modules which align in function and intent. Basically the motivation is to have a clue whats going on :-) 

## The Goal

The Goal of this repo is to define a logging system for use with the TwinCAT Event Logger, this uses the Tc_Message option so not a full alarm/event. This allows quick debuging style logging for during the development phase.

## Background

The background to this repo is essentially my leanring journey in PLC programming. Initially I had no strong view on how to construct a PLC program. As time has gone on I have learned OOP provides the best soltuion for architecting code.
This doesnt mean you must use full OOP, design patterns, testing etc, I believe you should, but its not required. Instead it means you simply divide the code into function, repeatable blocks, calling them classes or FBs doesnt matter.
The important part is you break up code into block and call those blocks cyclically, rather than in the structured programming paradigm.
Once you go donw this path, libraries like this start to make more sense. 
This library forms the basis of how i think those blocks of code should be constructed and operated.

## Description

The repo is effectively formed of a single object, TcMessage, this hosts a FB_TcMessage object from the event logger library. Using a single command you can send out a string message from any point in the code. In my own implementation I created a logger object in each of my program compoenents, but it would also work as a global singleton.

## Repository Design

The repo is split into 2 projects, the eventlog library and the testing project, the library is referenced in the test project. The test project can be run in the UmRT.

## Tests

There is a unit testing project created, the library is referenced in the test project. 

## Support

LOL, little old me now, all by myself :-)


## Requirements: 

Please include important requirements in the local readme files.

Currently nothing more than:

TwinCAT 4026


## Document List






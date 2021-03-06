## Development and Change Guidelines

This document describes the guidelines for ONVIF specification evolution. Its goal is to provide a transparent and open mechanism. 
The ONVIF Technical Committee implements the process described below when merging changes from internal or external contributors. 

## Specification Change Categories

Changes should fall into the following three categories:

* Clarification. The current description either doesn't make sense, is ambiguous, overly complicated, or unclear.

* Consistency. A portion of the specification is not consistent with the rest, or contraditcs to underlying specifications.

* New functionality. The proposal adds one or more features to the specifications.

## Specification Change Process

The change process depends on both the size and impact of the change proposal: 

Each change request (CR) affecting more than three lines of code shall be submitted as pull request. The comment of a pull request shall include the following information:
* Reason: containing a problem description and a description of the solution proposal.
* Compatibility analysis: An analysis describing possible impact on forward and or backward compatibility. 

As an exception to the above very small changes affecting no more than three consective lines may be filed as Issue including a reference to the affected code lines. Best create such issues by clicking on the affected code line or select those lines and use the "Reference in new issue" drop down menu left to the selection.

For larger additions affecting more than a simple type please see section "Feature Development Process" below.

## Specification workflow

ONVIF will maintain the following active branches:

* master - Current stable version.  
  No CRs are accepted directly to modify the specification.

* xx.nn - Development branch for next version  
  Change requests for clarifications and consistency may be submitted to this branch.
  Implementers may use this branch. However in the unlikely case of IPR notices indiviual changes may be revoked.

* xx.oo - Development branch for version after next version  
  Feature requests shall be submitted to this branch. Note that this branch will be frozen after about half a year for ONVIF IPR review.

Beside the above branches the following temporary branches may be established:  
* issue-xx-yyyyy - Change request for issue XX with short title YYYY.  
  Note that these branches may be deleted once the pull request has been approved.

* xxxx-yyyy - Feature branch for group xxxx with short title yyyyy.  

## Feature Development Process

New features shall not be developed on development branches but in separate feature branches. 
Feature branches may be part of the main ONVIF specification repository, but are typically located in separate repositories.

* Once an author or group has completed the specification development for a feature the respective feature needs to be verified by writing and executing test cases.
* When all activities have been completed the pull request shall include the following information:
  * Reason: containing a problem description and a description of the solution proposal.
  * Compatibility analysis: An analysis describing possible impact on forward and or backward compatibility. 
  * Unit tests covering the additional features
  * Information which parties implemented client and server side as well as a test report from at least two different entities.

## Tools

All documents are designed such that they can be edited by any text editor. Better use e.g. 
* Notepad++ www.notepad-plus-plus.org with XML Tools plugin for syntax checking. 
* Wysiwyg editing is supported by
  * Oxygen www.oxygenxml.com
  * XMLmind www.xmlmind.com/xmleditor/download.shtml
    Be careful when using this editor because it tends to reformat the complete document. Usage for creating snippets is ok.

For text documents DocBook5 is used. For details on DocBook editing and formatting see https://docbook.org/ .
## Maintainers

The elected ONVIF Technical Committee members act as change control board and maintainers of this repository. Typically any change proposals is kept pending for at least two weeks to collect comments. Decisions on pull requests and issues will be documented in place. 

Note that this repository sole purpose is technical specification evolution. Any possible product incompatiblities must be directed to vendors. 

## Participation

While governance of the specification is the role of the ONVIF Technical Committee, the evolution of the specification happens through the participation of members of the developer community at large. 
Any person willing to contribute to the effort is welcome, and contributions may include filing or participating in issues, creating pull requests, or helping others with such activities.


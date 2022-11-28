# RTaW-Pegase YANG-XML Export

This folder contains the list of YANG modules to which [RTaW-Pegase](www.realtimeatwork.com/rtaw-pegase/) YANG-XML export complies.
These modules are :

 - IETF standards-track YANG modules
 - IEEE experimental YANG modules
 - RTaW-specific YANG modules

Following changes were made in modules in order to solve Sysrepo import issues
 - ieee802-dot1q-types : obsolete is not recognized, obsolete grouping type removed and new grouping renamed
 - ieee802-dot1q-bridge : addede some missing prefixes
 - ieee802-dot1q-sched : removed some 'must' checks comparison on fractional-grouping seems not supported, added some missing prefixes
 - ieee802-dot1q-psfp :  removed some 'must' checks comparison on fractional-grouping seems not supported, added some missing prefixes

These changes were communicated to IEEE yangsters.
# Change log
RTaW-Pegase 4.3
 - added AS2020 yang module for information, not yet used in exports, it references ieee1588 modules
 - rtaw-network-topology : added documentation, unit for speed, speed type changed to uint32
 - rtaw-routing : remove redundant information
 - rtaw-streams : add missing size for induced stream type
RTaW-Pegase 4.2.6
 - added static routing tables documentation
 - add missing req/resp frames in DialogOverEthernet
 - typo nodeAllocatedTo in rtaw-network-topology.yang

RTaW-Pegase 4.2.4
 - fix on rtaw-streams model

RTaW-Pegase 4.2.1
 - extended rtaw-stream to support tftp, tcp dialog over tcp com patterns
 - new rtaw-services module to describe RTaW SomeIP services

Pegase 4.1.5
 - moved to latests standards for ieee802-dot1q-preemption.yang, iana-if-type.yang,
 - revert changes in ietf-interfaces.yang to use published version,
 - moved cbs module as RTaW vendor specific module.
 
# YANG models Directory Structure
The directory structure is as follows

 - **standard** : contains standards-track YANG modules
 - **standard/ieee** : standard modules (published or drafts) intended for IEEE submission.
 - **standard/ietf**: standard IETF YANG modules
- **standard/iana**: standard IANA YANG modules
- **vendor**: contains vendor-specific YANG modules
- **vendor/rtaw**: [RTaW](www.realtimeatwork.com) YANG modules
- **scripts**: utilities for Sysrepo configuration 


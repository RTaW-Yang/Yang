# Yang

This repository contains the list of Yang modules to which [RTaW-Pegase](www.realtimeatwork.com/rtaw-pegase/) and [TSN-Configurator](https://tsn.studio) YANG-XML export complies.



Structure of the repository
 - **ieee**: standard modules (published or drafts) intended for IEEE submission
 - **ietf**: standard IETF YANG modules
 - **iana**: standard IANA YANG modules
 - **rtaw**: [RTaW](www.realtimeatwork.com) specific YANG modules

# RTaW specific modules
- **cbs**: module specifying idle slope configuraiton on output port queues.
- **streams**: module specifying streams on a network .
- **routing**: module specifying routing of streams on a network .
- **extensions**: extensions to standard module in the.

# Change log
Following changes were made in modules in order to solve Sysrepo import issues, the changes are highlighted in the yang modules as well.

 - ieee802-dot1q-types : obsolete is not recognized, obsolete grouping type removed and new grouping renamed
 - ieee802-dot1q-bridge : added some missing prefixes
 - ieee802-dot1q-sched : removed some 'must' checks comparison on fractional-grouping seems not supported, added some missing prefixes
 - ieee802-dot1q-psfp :  removed some 'must' checks comparison on fractional-grouping seems not supported, added some missing prefixes

# Contact
contact@realtimeatwork.com



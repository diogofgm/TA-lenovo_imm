=============
Configuration
=============

Splunk
------
- Configure a new index (e.g. imm) for the new logs

Receiving syslogs on Splunk
~~~~~~~~~~~~~~~~~~~~~~~~~~~
NOTE: Its recommended to use a separate and dedicated syslog solution (e.g. rsyslog, syslog-ng, etc)
- Configure new UDP port (e.g. 514) pointing to the new index using the "lenovo:imm" sourcetype

Monitoring log files
~~~~~~~~~~~~~~~~~~~~
- Configure a new file monitor input pointing to the new index using the "lenovo:imm" sourcetype

Lenovo IMM
----------
- Configure syslog outputs
For more information please refer to the `Lenovo IMM documentation`_ or `Lenovo IMM user guide`_.



.. _Lenovo IMM documentation: https://systemx.lenovofiles.com/help/index.jsp
.. _Lenovo IMM user guide: https://download.lenovo.com/ibmdl/pub/pc/pccbbs/thinkservers/imm_userguide.pdf
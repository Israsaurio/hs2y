Will write later :D  HS2TY!!!!

Dev Database Layout (MongoDB):

**DB**
  * test

**Tables**
  * Pots: Honey pots (HTTP, FTP, SMTP, etc...)
    * ID: pre-assigned ID via Mongo for records
    * Name: name of honey pot
    * Port: port HP uses
  * Rules: any rules (regex-compatible) to compare incoming data with
  * Actions: what to do when a rule is matched
  * Flies: Log of attempts/connections

**Notes**
Each action is tied to a rule, and each rule is tied to a honey pot based on ID.
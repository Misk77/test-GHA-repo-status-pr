This is for testing slack bot with different slack notification.
---

Requires: 
Auth for chat_write on slack app
- OAuth & Permissions > scope


secrets for repo
- BOT
- URL


# READ THIS!
PROD user/application credentials:
#solace enters the password in #solace ansible vault but developers are responsible for posting it in their own sealed secrets in gitops,.
This sealed secrets is requested by developers directly to #sysman-linux


Service type: Production Secrets "Helm"
Request link:
http://vltcordw01.test1.hh.atg.se/index.php


respectMsgPriorityEnabled:
Existing queue need to be shutdown before this value can be changed.
This means, before the repo is merged or as for PROD,  before a release is manually trigged in go-pipeline.“respectMsgPriorityEnabled: Flows must be shutdown prior to changing the respect for message priority”

 - Otherwise the pipeline will fail and no changes will be done.

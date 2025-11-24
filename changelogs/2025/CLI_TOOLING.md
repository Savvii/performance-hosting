# Changelog

## 202505080807 - 08/05/2025
- Added the `dbug` tool to our tooling arsenal.
- Added the `mnage` tool to our tooling arsenal.

## 202505151758 - 15/05/2025
- Removed our old `savvii` tool.
- Created a fallback for several commands to `mnage` for backwards (CI) compatibility.

## 202505191435 - 19/05/2025
- Added JSON formatting to our DB `dbug` commands.
- Fixed a namespacing bug in our SSL `mnage` commands that only gets triggered after packaging.

## 202506131525 - 13/06/2025
- Added a feature to check all present domains for Letsencrypt validation instead of only new domains. This fixes questions and confusion when being unable to add a new domain.
- Fixed a bug in the `db:slowlog` command output
- Fixed a bug in the `db:locks` command output
- Refactored error handling

## 202511242113 - 24/11/2025
- Added `mnage vhost:alias` commands to add/list and delete vhost aliases for shared server setups
- Added `mnage cron` commands to add/list and delete cronjobs
- Added `mnage ipblock:remove` command to remove an ip from the firewall blocklist (set by Fail2Ban)
- Added `mnage superviser:enable` command to enable Supervisor (Process Control System)
- Added `mnage services` commands to list and restart services running in userspace
- Fixed a bug in the `dbug search:stats` command, so it support OpenSearch

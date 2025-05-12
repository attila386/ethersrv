# Sync code from DOS machine to Git

What about if you can develop software (or anything else) on your retro DOS PC
and to be able to transfer it to github with ease?

For the story visit my [website](https://socket7.hu).

Scripts:

- nd-ethersrv : for starting up ethersrv
- nd-sync : for syncing the shared folder
- nd-shutdown : initiate shutdown of

Units:

- nd-ethersrv.service : runs nd-ethersrv at system startup
- nd-shutdown.service : runs nd-shutdown script
- nd-shutdown.timer : schedule nd-shutdown service
- nd-sync.service : runs nd-sync script
- nd-sync.timer : schedule nd-sync service

Logrotate:

Sets up policy to rotate log created by scripts.

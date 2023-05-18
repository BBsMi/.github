# BBsMi
A Retro BBS Suite for Linux and Unix Hosts

## Goals
- [ ] Truecolor support
- [ ] Sixtel support
- [ ] Animation support
- [ ] SSH wrapped session
- [x] Turnkey menu module
- [ ] Userbased WebDAV Suitcase support (Upload, Share, Download files)
- [ ] Multiuser games (A day at the race conditions, Legend of the Red Dragon, MajorMUD, Tradewars, and more)
- [ ] Text browser support

## Projects

### [SerenadeMi](//github.com/BBsMi/SerenadeMi)
Turnkey menu module for building BBsMi apps

### [ShellMi](//github.com/BBsMi/ShellMi)
User shell for BBsMi users

### [AdminMi](//github.com/BBsMi/AdminMi)
Administration and Management CLI for BBsMi

### [ServeMi](//github.com/BBsMi/ServeMi)
Turnkey web server for BBsMi

## Basics
BBsMi relies heavily upon SSH and normal Linux / Unix user management. Anything that PAM can use as a backend, we can use

BBsMi has five distinct user groups:

### bbsmi-admins
Special backend access only used for administration and maintence.


### bbsmi-staff
Users with some administration tasks.

### bbsmi-pusers
Power (paid) users. Users that are allowed more time in a day.

### bbsmi-rusers
Regular (unpaid) users. Standard user pool.

### bbsmi-guests
Guests (Unverified) users. This is where every user except admins start

## License
[(c) 2023 GNU AFFERO GENERAL PUBLIC LICENSE v3.0](//github.com/BBsMi/.github/blob/trunk/LICENSE)

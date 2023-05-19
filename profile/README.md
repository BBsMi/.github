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
 - [ ] Truecolor support
 - [ ] Sixtel support
 - [ ] Possible virtual terminal / split screen support via Screen or Tmux
 - [ ] Replace standard user shell
 - [ ] VT100/VT220 fallback support
 - [ ] File transfer suppport

### [AdminMi](//github.com/BBsMi/AdminMi)
Administration and Management CLI for BBsMi
 - [ ] Status dashboards
 - [ ] User management
 - [ ] Package management
 - [ ] Maintence management


### [ServeMi](//github.com/BBsMi/ServeMi)
Turnkey web server for BBsMi
 - [ ] New user registration
 - [ ] WebDAV personal suitcase
 - [ ] Manage SSH keys
 - [ ] User profiles
 - [ ] Content Management System
 - [ ] Payment gateway
 - [ ] (Admin) User management

## Basics
BBsMi relies heavily upon SSH and normal Linux / Unix user management. Anything that PAM can use as a backend, we can use

BBsMi user UIDs start at 50000 and go down by one. A user has their username as their primary group; uid / gid match or skip to next number down and then are added to the proper group. BBsMi applications by design will interface with a user based on their highest attached user group only.

BBsMi has six distinct user groups:

### bbsmi-admins
GID 55555. Special backend access only used for administration and maintence.

### bbsmi-staff
GID 44444. Users with some administration tasks.

### bbsmi-pusers
GID 33333. Power (paid) users. Users that are allowed more time in a day.

### bbsmi-rusers
GID 22222. Regular (unpaid) users. Standard user pool.

### bbsmi-guests
GID 11111. Guests (Unverified) users. This is where every user except admins start

### bbsmi-banned
GID 6666. Users that may never login again and usernames that may never bereused

## License
[(c) 2023 GNU AFFERO GENERAL PUBLIC LICENSE v3.0](//github.com/BBsMi/.github/blob/trunk/LICENSE)

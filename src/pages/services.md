# Overview

The network has three active service entities:

* NickServ
* ChanServ
* MemoServ

General help info can be requested by messaging 'help' to any of them.

## Usage examples

Terminology: words in <> are mandatory arguments.
Ones in [] are optional. Both should be typed in without the brackets.

### Nickserv

Nick registration:

	msg nickserv register <password> [email]

Identification:

	msg nickserv identify <password>

### ChanServ

Channel registration:

	msg chanserv register <channel> [description]

That will register the channel to your previously registered nick.
You cannot register channels without being registered *and* identified
with NickServ.

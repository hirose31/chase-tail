# NAME

__chase-tail__ - notify and cosmetic log lines

# SYNOPSIS

__chase-tail__ [ -d ]
[ --max-lps|-l max_lps ]
[ --flood-message|-m flood_message ]
[ --log-type|-t log_type ]

    $ tail -F access_log | chase-tail -l 10 -t http_error

# DESCRIPTION

notify and cosmetic log lines.

# OPTIONS

- --max-lps | -l max_lps:Int

if number of lines in a second exceeds this max_lps, print flood message into STDERR.

default is fixme.

- --flood-message | -m flood_message:Str

default is "NOTIFY_FLOOD".

it is good idea that you set this message as trigger of iTerm2 (Profiles -> Advanced -> Triggers).

- --log-type | -t log_type:Str

specify log type for cosmetic log lines.

default is "plain" that is no cook up just return it.

- -d
- __--debug__

increase debug level.
-d -d more verbosely.

# AUTHOR

HIROSE, Masaaki <hirose31 _at_ gmail.com>

# COPYRIGHT & LICENSE

This program is free software; you can redistribute it and/or modify it
under the same terms as Perl itself.
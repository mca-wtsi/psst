# NAME

App::psst - prompt string setting tool

# DESCRIPTION

Set-once configuration for `~/.bashrc` to show presence of
`$PERL_LOCAL_LIB_ROOT`.

## Origin

I wrote a [local::lib](http://search.cpan.org/perldoc?local::lib)-based installer for a small project.

I added the obligatory "set up the environment and start a shell in
there" script.

I wanted the new subshell to be clearly marked as having local::lib
environment, and decided that this functionality doesn't belong in the
small project.

## Intentions

Polish it a little to make a small CPAN-installable package.  Install
in all my $HOMEs.



# AUTHOR

Copyright (C) 2011 Genome Research Limited

Author Matthew Astley L<mca@sanger.ac.uk>

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

## Thanks

Thanks to Magnus Manske for some useful discussion of the mechanism,

and this post for convincing me that this is a useful route to sanity
http://blogs.perl.org/users/oliver_gorwits/2011/07/locallibs-for-dist-development.html

and to my employer for making it easy to mix free software with $work.



# SEE ALSO

L<psst(1)>

## Related tools

These are tools I have found links to.  I have not yet chosen some to
assemble a better working environment.

- [Git::CPAN::Hook](http://search.cpan.org/perldoc?Git::CPAN::Hook) or [CPANPLUS::Dist::GitHook](http://search.cpan.org/perldoc?CPANPLUS::Dist::GitHook)
- [App::local::lib::helper](http://search.cpan.org/perldoc?App::local::lib::helper) ([App::local::lib::helper::rationale](http://search.cpan.org/perldoc?App::local::lib::helper::rationale))

`localenv bash` starts a new shell, which psst can configure.

- [App::PerlLocalEnv](http://search.cpan.org/perldoc?App::PerlLocalEnv), L<perl-local-env(1)>

`perl-local-lib $DIR activate` starts a new shell, which psst can
configure.

- [App::local::lib::Win32Helper](http://search.cpan.org/perldoc?App::local::lib::Win32Helper)

This psst has not (yet) been tested with bash under Windows.

- [App::perlbrew](http://search.cpan.org/perldoc?App::perlbrew)

This version of psst knows nothing about perlbrew.
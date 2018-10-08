:Date: 2018-10-08
:Version: 18.9b0
:Copyright: 2018 Åukasz Langa
:Title: black
:subtitle: uncompromising Python code formatter
:Manual section: 1

Description
============

``black`` is the uncompromising Python code formatter.

Summary
#######

``black`` is the uncompromising Python code formatter. By using it,
you  agree to cede control over minutiae of hand-formatting. In return,
Black gives you speed, determinism, and freedom from pycodestyle
nagging about formatting. You will save time and mental energy for
more important matters.

Usage
#####

black [OPTIONS] [SRC]...

Common Options
##############

Options:

::

  -l, --line-length INTEGER       How many characters per line to allow.
                                  [default: 88]

  --py36                          Allow using Python 3.6-only syntax on all
                                  input files.  This will put trailing commas
                                  in function signatures and calls also after
                                  *args and **kwargs.  [default: per-file
                                  auto-detection]

  --pyi                           Format all input files like typing stubs
                                  regardless of file extension (useful when
                                  piping source on standard input).

  -S, --skip-string-normalization
                                  Don't normalize string quotes or prefixes.

  --check                         Don't write the files back, just return the
                                  status.  Return code 0 means nothing would
                                  change.  Return code 1 means some files
                                  would be reformatted.  Return code 123 means
                                  there was an internal error.

  --diff                          Don't write the files back, just output a
                                  diff for each file on stdout.

  --fast / --safe                 If --fast given, skip temporary sanity
                                  checks. [default: --safe]

  --include TEXT                  A regular expression that matches files and
                                  directories that should be included on
                                  recursive searches.  An empty value means
                                  all files are included regardless of the
                                  name.  Use forward slashes for directories
                                  on all platforms (Windows, too).  Exclusions
                                  are calculated first, inclusions later.
                                  [default: \.pyi?$]

  --exclude TEXT                  A regular expression that matches files and
                                  directories that should be excluded on
                                  recursive searches.  An empty value means no
                                  paths are excluded. Use forward slashes for
                                  directories on all platforms (Windows, too).
                                  Exclusions are calculated first, inclusions
                                  later.  [default: /(\.git|\.hg|\.mypy_cache|
                                  \.tox|\.venv|_build|buck-out|build|dist)/]

  -q, --quiet                     Don't emit non-error messages to stderr.
                                  Errors are still emitted, silence those with
                                  2>/dev/null.

  -v, --verbose                   Also emit messages to stderr about files
                                  that were not changed or were ignored due to
                                  --exclude=.

  --version                       Show the version and exit.

  --config FILE                   Read configuration from PATH.

  -h, --help                      Show this message and exit.

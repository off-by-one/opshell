# opshell

Helper shell for the [1password
CLI](https://support.1password.com/command-line-getting-started/). This will
manage your signin and signout, and give some helper functions for common
actions.

## Prerequisites
  - [op cli](https://app-updates.agilebits.com/product_history/CLI)
  - [pwgen](https://linux.die.net/man/1/pwgen)

## Usage

```
$ opshell
Enter the password for <account> at <subdomain>.1password.com:
Welcome to the 1password subshell!

 - op     [command...]  | execute a 1password command in this session
 - opwgen [item] [opts] | use pwgen flags to generate a password
 - opexit               | use op signout to securely exit the session
op | $ op get item "test account"
{...}
op | $ opwgen "test account" -A0 10
op | $ opexit
exit
$ opshell opwgen "test account" -A0 20
Enter the password for <account> at <subdomain>.1password.com:


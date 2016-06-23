Disable login errors
====================

Prevent the display of all login error messages. A user attempting to login will
not be aware if the account exists, an invalid user name or password has been
submitted, or if the account is blocked. Some of the messages which are hidden
include:

* _Sorry, unrecognized username_
* _Sorry, incorrect password_
* _Sorry, [username] is not recognized as a user name or an e-mail address._
* _The account for [username] has not been activated or is blocked._
* _Sorry, there have been more than 5 failed login attempts for this account. It is temporarily blocked. Try again later or request a new password._

This module mitigates a vector to collect a set of valid usernames by
interacting with the login forms. It hampers attempts to use brute
force testing, in which the tester verifies if, given a valid username, it is
possible to find the corresponding password.

Use of this module is meant to toughen against the username enumeration test
cases found in the OWASP Testing Guide Project,
Testing for User Enumeration and Guessable User Account
([OWASP-AT-002](https://www.owasp.org/index.php/Testing_for_User_Enumeration_and_Guessable_User_Account_(OWASP-AT-002))).

Current Maintainer
------------------

- David Norman (https://github.com/deekayen)

Credits
-------

- Originally added by David Norman to Drupal's Login Security module
  (https://www.drupal.org/project/login_security)
- Ported to Backdrop by David Norman (https://github.com/deekayen)

License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.

# SafeOTP
A basic Android authenticator app that encrypts the private keys with a pin or passphrase.

* Current Status
Pre-initial version. At this point, SafeOTP is a simple clone of FreeOTP. _Stay tuned....._

## Design
In order to add or view the OTP a password will be required.
* Each private key will be encrypetd by a provided passphrase.

### Security Considerations
Using a short passphrase is very prone to a brute-force attack, however, it is difficult to enter a long passphrase on a touch-screen. To mitigate this problem I am taking a slightly unconventional approach....
* When an invalid passphrase is provided it will be accepted by the app, but the resulting OTP will not be valid.
   * To avoid typos I will take the enterred pin/passphrase and generate some kind of graphic that will help
     the user recognize when they have enterred the correct value.

## Branches
### Branch: upstream
The upstream branch will track the FreeOTP project at fedorahosted.org:
* https://fedorahosted.org/freeotp/
* git://git.fedorahosted.org/freeotp/android.git

### Branch: hacking
Work in progress. Note that I may rebase this branch or rewrite history.

### Branch: master
I will try and keep this branch reasonably stable.

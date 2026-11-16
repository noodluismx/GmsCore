# Solution for Issue #2851: [BOUNTY] Support Play Integrity over remote DroidGuard + Server/Guide [$85]

Play Integrity should be supported over the _remote DroidGuard_ functionality and there should be documentation how to set up a phone as a DroidGuard server.

**Why?**
While existing solutions allow getting a sufficiently passing Play Integrity token with a non-integrity-compliant device, there is the following problems that come with it:
- the requirement for a rooted phone,
- running the integrity-checking code from google on your phone that's purposefully obfuscated and fetched at runtime,
- running strange bypassing software with root permissions, like the closed-source TrickyStore and
- all of this has to permanently be kept up-to-date in line with updates to Play Integrity to stay passing

This is tedious, never-ending work that everyone rather avoids.
If you're a busy person it's also not really feasible. Imagine coming out of a cinema with your friends and heading for a rentable scooter only to realize you're device doesn't pass Play Integrity anymore.

If PI would work over another device, like an old, stock one you still have at home, it would fix these problems.
It would also open the oppurtunity for commercial integrity-attestation offerings, where you would like pay monthly and they then allow you to use their devices over a server which then serves valid integrity tokens to your device.

**How to implement?**
- [ ] Fix:
  > remote droidguard currently does not work for play integrity due to play integrity using a multi step droidguard process and the implementat

## Build Terminologies

### Day-Build
* Purpose: Give feedback to developer developing code as early as possible
* Approach: 
    * Build on every change (feasible only for small teams & when build time is less)
    * Build periodically during the day (every 1 hour)
* What we do w.r.t Tests
    * Unit Tests
    * Smoke Tests 
* What else
    * Code Quality

### Nightly-Builds
* Purpose: For Testing/Other teams to use stable set of features/issue fixed
* Approach:
    * Build only once per day (Daily night @ 11pm )
* What tests do we execute
    * Unit Test
    * System Tests 
    * Performance Tests
* What else
    * Code Quality
    * Push our binaries to remote repositories like artifactory/Nexus

* If it fails make noice
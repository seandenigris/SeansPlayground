# Introduction #

You want to say something like, "pretend it's 1/1/2013 @ 9am". How do you say that? You need to intercept something. Where do you intervene?

## Options: ##
### myObject>>#now - like the Ultra Thin GUI pattern ###
  * Pro: no implementation details exposed (e.g. that we're sending #now to DateAndTime)
  * Con: we're not testing that the message gets sent e.g. that we have a one-liner #now ^ DateAndTime now

### DateAndTime>>#now ###
  * Pro: This presumably would be tested by the core and have lots of eyes on it, so as long as we know it's being called, we can be confident that all our behavior is tested
  * Con: Now we have duplicated the system logic in the test i.e. the test knows we're calling DateAndTime>>#now, so it must be changed in two places. Theoretically, we could say (pseudo-code) ^ DateAndTime date: Date today time: Time now, and although the code might still be working, the test would fail

### Hand-written double ###
We could start to build a double for DateAndTime where you could pretend it's a specific time and then implement the common messages to all return the expected result, or more generally a way to change the timestamp for the whole system e.g. in Date and Time too
## August 3

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)


### 2.8 release

* The beta 4 waits for the next TTK beta release, which has been delayed.


### Potential stability issue in master

* It's been reported that latest changes in master have potential problems with
  migrations.
* Is master stable?
* A fix is in the works. If it doesn't arrive quick enough, reverting some
  conflictive commits might be an option.


### Some regressions

* Following the fix to unmute quality checks
  ([#5010](https://github.com/translate/pootle/issues/5010)), it seems like
  there's some regression when it comes to muting non-critical checks
  ([#5013](https://github.com/translate/pootle/issues/5013)).
* Going through a particular filter while performing actions that affect such
  filter still result in a situation where users cannot go further
  ([#4983](https://github.com/translate/pootle/issues/4983)).
  [MLO](https://mozilla.locamotion.org) seems to have exhibited this too,
  although it's running many commits behind master.


### Next triage meeting

Wednesday, 10th of August, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/10).

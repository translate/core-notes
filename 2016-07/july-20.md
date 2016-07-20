## July 20

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)


### 2.8 release

* The hard deadline for 2.8 final (which was due at the end of July) will rather
  be a soft one.
* Beta needs more testing and exposure to users, however it's been difficult to
  have people test it, as they are having trouble to upgrade from older
  versions.
* Pushing TTK2 to Beta users will also allow to test TTK2 in other environments
  more thoroughly. In case it's not stable enough yet, the decision can be
  reverted ([#4914](https://github.com/translate/pootle/pull/4914)).
* The issue with the editor JS leaks is a blocker
  ([#4916](https://github.com/translate/pootle/issues/4916)).
* Ideally a new beta release will come out tomorrow.


### Ongoing work

* [Taras](https://github.com/ta2-1) is working on expanded stats tables
  ([#4926](https://github.com/translate/pootle/issues/4926)) and top
  contributors list ([#4868](https://github.com/translate/pootle/pull/4868)).
* [Leandro](https://github.com/unho) is working on RTL and localizability issues
  ([#4925](https://github.com/translate/pootle/issues/4925),
  [#4923](https://github.com/translate/pootle/issues/4923)).


### JS memory leaks

* The editor leaks memory over time when navigating through units.
* What's specifically leaking? Event listeners get back to normal after garbage
  collection, however the amount of DOM nodes (and as a consequence the total
  memory heap size) doesn't shrink enough to expected values.
* Leakage patterns can be various, including library bugs, using globals in
  jQuery event listener callbacks and more.
* Leakage might happen either when redrawing the editor table, or when routing
  through the callback used in the jQuery-history plugin (`$.history.init()`).
* A potential way to determine the root cause will be disabling internal
  components. [Ryan](https://github.com/phlax) already tried to disable external
  components and also fixed an array leakage in the `fetch()` utility
  ([#4920](https://github.com/translate/pootle/pull/4920)).


### Next triage meeting

Wednesday, 27th of July, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/8).

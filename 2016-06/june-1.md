## June 1

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)

### 2.8 release

* Work on Pootle FS is not finished yet, the major bits are expected to be done
  by the end of this week. MLO will be updated with this and a beta will come
  after.
* [Taras](https://github.com/ta2-1) is working on adding the translated
  wordcount to `ScoreLog` models
  ([#4761](https://github.com/translate/pootle/issues/4761)).
* The issue to clarify the display of empty resources seems to be stalled. Since
  there are specific suggestions, addressing the reported core issue (feeling of
  brokeness) should be trivial
  [#4748](https://github.com/translate/pootle/issues/4748).

### Ongoing work

* Work on the raw font PR continues to address the remaining issues. Integrating
  CodeMirror didn't solve the undo-related problems and a simple custom stack
  has been written ([#4171](https://github.com/translate/pootle/pull/4171)).

### Triaging

#### Assigned to 2.8

* Displaying of errors for external XHR requests will be adjusted
  ([#4771](https://github.com/translate/pootle/issues/4771)).

#### Pushed for the next cycle

* [Splitting submission
  types](https://github.com/translate/pootle/wiki/Splitting-SubmissionType-into-SubmissionSource-and-SubmissionAction)
  to distinguish units created via uploads will be needed once `pootle_fs` is in
  place ([#4774](https://github.com/translate/pootle/issues/4774)).

### Next triage meeting

Wednesday 8th of June, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/2).

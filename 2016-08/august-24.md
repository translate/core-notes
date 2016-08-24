## August 24

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)


### Updates

* 2.8.0 Beta 4 tentatively out at end of the week.
* Pinning to specific versions of dependencies seems to have good acceptance
  ([#5133](https://github.com/translate/pootle/issues/5133)).


### Store-related changes

- It might be a false alarm (and it's easy to confuse things due to having the
  TTK base storage class mixed into the Store model), but it might be that
  context is not used correctly when getting unitid
  ([#5109](https://github.com/translate/pootle/issues/5109)).
- Setting the same revision to the unsynced units being updated, seems to
  provide some performance improvements in testing scenarios
  ([#5147](https://github.com/translate/pootle/pull/5147)).
- Denormalizing `get_max_unit_revision()` will considerably reduce the queries
  done to retrieve the maximum revision number
  ([#5146](https://github.com/translate/pootle/pull/5146)). Taras would like to
  check possible scenarios to be 100% sure this does the same thing as before.
- Factoring out model methods to other classes can help with migration testing,
  as Django migrations are constained to using the data of a model at a specific
  point in time, and its methods are not available there.


### Next triage meeting

Wednesday, 31st of August, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/13).

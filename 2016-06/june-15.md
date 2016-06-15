## June 15

### Attendees

* [Leandro](https://github.com/unho) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)

### 2.8 release

* First beta is expected by end of week. `pootle_fs` needs to be landed and
  some major bugs in 2.8.0 milestone still need to be fixed.

### Triaging

Quite a bit new issues this week.

#### Assigned to 2.8

* Reposition Last updated column in stats table
  ([#4817](https://github.com/translate/pootle/issues/4817)).
* Add more tests for contributors command
  ([#4797](https://github.com/translate/pootle/issues/4797)).
* JS client sends CSRF headers in external requests
  ([#4808](https://github.com/translate/pootle/issues/4808)).
* Add --until to contributors command
  ([#4816](https://github.com/translate/pootle/issues/4816)).
* Avoid HTML markup in Entire project content dropdown
  ([#4820](https://github.com/translate/pootle/issues/4820)).


#### Pushed for the next cycle

* Download of formats other than PO don't allow upload in anything but PO
  ([#4790](https://github.com/translate/pootle/issues/4790)).
* Eliminate errors from `setup.py build_mo --all`
  ([#4791](https://github.com/translate/pootle/issues/4791)).
* update_tmserver should page through retrieved data
  ([#4792](https://github.com/translate/pootle/issues/4792)).
* Sometimes "Back" button in browser doesn't work
  ([#4793](https://github.com/translate/pootle/issues/4793)).
* Update timeline tests to ensure that it doesnt fail on units with no creation
  time ([#4807](https://github.com/translate/pootle/issues/4807)).
* Due dates:
  * Implement Due Dates functionality
    ([#4799](https://github.com/translate/pootle/issues/4799)).
  * Define `DueDate` model
    ([#4800](https://github.com/translate/pootle/issues/4800)).
  * Add Due Dates widget in browsing pages
    ([#4801](https://github.com/translate/pootle/issues/4801)).
  * Implement Due Dates dashboard
    ([#4802](https://github.com/translate/pootle/issues/4802)).
  * Implement Due Dates notification emails
    ([#4803](https://github.com/translate/pootle/issues/4803)).
  * Implement Due Dates admin dashboard
    ([#4804](https://github.com/translate/pootle/issues/4804)).


### Next triage meeting

Wednesday 22nd of June, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/4).

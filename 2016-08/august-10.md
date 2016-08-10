## August 10

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)


### Releases

* [Translate Toolkit beta
  4](https://github.com/translate/translate/releases/tag/2.0.0b4) has been
  released.
* In the best-case scenario, Pootle 2.8.0 beta 4 should be available by the end
  of the week.

#### Structural changes during beta releases

* Monolingual file format support and allowing multiple file types per project
  is quite an invasive change for a product in beta cycle.
* This shouldn't be the case again. This has been an exception to allow bringing
  deployments in 2.5 up to 2.8. Without this feature, they couldn't upgrade
  without missing on features available in 2.5.
* The end goal is bringing as many people as possible onto 2.8.
* Once all of these changes have been merged, work should focus on stabilization
  towards the final release.
* With 2.8 out, 2.5 becomes obsolete. What's the approach to obsoleting
  releases? It seems a bit unclear, Dwayne might be able to shed some light.


### Notifications

* Notifying users when a comment has been added while reviewing a suggestion can
  not only be benefitial, but is an immediate need
  ([#5401](https://github.com/translate/pootle/issues/5041)).
* While this can be implemented with an ad-hoc solution, notifications as a
  whole need more thought.
* GitHub-style subscription to notifications might work, when an action taken on
  an item will automatically subscribe the user to any notification for future
  changes performed on such item.
* Due Dates will also need from notifications.


### Editor with raw font

* Unit tests have been added to the branch which fixes issues with escaped
  characters by leveraging a custom raw font
  ([#4171](https://github.com/translate/pootle/pull/4171)).
* Evernote will deploy off this branch to production early next week. Based on
  the feedback received during that time, it'll be ready to be merged to master
  or not.


### Next triage meeting

Wednesday, 17th of August, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/11).

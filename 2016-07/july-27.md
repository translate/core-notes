## July 27

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)


### 2.8 release

* [Beta 3 was out last
  week](https://github.com/translate/pootle/releases/tag/2.8.0b3). Also [TTK2
  beta 3 is out](https://github.com/translate/translate/releases/tag/2.0.0b3).
* Beta 4 coming out soon.
* Some upcoming tasks for a 2.8 release might not have immediate fixes.
* Some invasive changes upcoming as part of beta to support multiple formats per
  project ([#4929](https://github.com/translate/pootle/issues/4929)) and
  monolingual file formats
  ([#4957](https://github.com/translate/pootle/issues/4957)).


### Ongoing work

* Retrieving user's last events is expensive. Adding a LRU cache will definitely
  help ([#4974](https://github.com/translate/pootle/pull/4974)), although
  denormalizing might be best
  ([#4975](https://github.com/translate/pootle/issues/4975)).
* Some localizability issues will be addressed as soon as possible
  ([#4933](https://github.com/translate/pootle/issues/4933),
  [#4934](https://github.com/translate/pootle/issues/4934)).


### Robots and performance

* There's been some early discussion around the impact of robots on performance
  ([#4977](https://github.com/translate/pootle/issues/4977)).
* This is mostly affecting pages which include user statistics. These pages are
  not visited often by humans, but frequently by robots.
* Probably only logged-in users should have access to user's statistics
* As a related thought, user's latest activity might leak activity from projects
  inaccessible/hidden to others.


### Next triage meeting

Wednesday, 3rd of August, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/9).

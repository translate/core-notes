## July 13

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)


### 2.8 release

* Whatever gets in by the end of the week will become part of Beta2, which
  should by out by next Monday.
* There's a regression in browsing pages where on the first page load the stats
  table will be filed only after a delay. This seems to happen only in Chrome
  however it would be great to have this fixed by 2.8.0.
  ([#4885](https://github.com/translate/pootle/issues/4885)).
* Truncating names in the browsing tables has been implemented
  ([#4883](https://github.com/translate/pootle/pull/4883)), although
  [Leandro](https://github.com/unho) is unsure about the approach and would love
  to hear more thoughts on that before the end of the week if possible.
  * Regarding the original issue
    ([#4817](https://github.com/translate/pootle/issues/4817)), it's been
    stressed that there is no consensus on repositioning columns, so while
    there's no agreement, no change will happen.
* Working towards making virtual folders a plugin is still on the radar
  ([#4650](https://github.com/translate/pootle/pull/4650)), although not a
  blocker on its own. The main objective is setting a baseline for writing
  plugins.


### Next triage meeting

Wednesday, 20th of July, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/7).

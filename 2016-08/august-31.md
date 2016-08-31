## August 31

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)


### 2.8 release

* It will probably be delayed a bit. It needs more real world testing.


### Invasive changes

* The invasive PR changes being merged to master are split so they are easier to
  review on their own.
* These PRs don't trigger any new functionality on their own.
* In terms of test coverage, master's situation is way better than 6 months ago.
* Test coverage doesn't necessarily guarantee proper functioning of the entire
  system though, and bugs can always slip in. It's inevitable.
* Translate House cannot take responsibility of all the effects of the code
  (also per the GPL), and stresses Evernote to do its own due diligence.

#### On stability

* Evernote's fundamental requirement is to keep their mission critical
  infrastructure stable, and master being stable is part of that.
* It seems like there is a disagreement on what master being stable means;
  expectations might vary across teams, development pace definitely does.
* There are also doubts on how (major) changes are being approached.
* Evernote is still on the opinion that the specific [major changes taking place
  right now](https://github.com/translate/pootle/pull/5161) would better be on a
  separate branch.

* People need to keep working but some interested parties have been out of this
  discussion. It might be better to follow-up that conversation on other
  channels.


### Next triage meeting

Wednesday, 7th of September, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/14).

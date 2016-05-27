## May 27

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)

### 2.8 release

* [Ryan](https://github.com/phlax) is working on finalizing the last bits of
  `pootle_fs`, and hopes to have it ready by early next week.
* A beta will be released quickly after. A few betas can be expected before
  2.8.0 final is out, as this includes work from the past ~6 months.
* Once `pootle_fs` lands, [Ryan](https://github.com/phlax) will take care of the
  editor-related regressions. These fixes are needed by Evernote to update their
  deployment.
* There's also the desire to have the externalized virtual folder code be part
  of the 2.8.0 release, as that will allow other developers to grasp how to
  create external plugins (PRs
  [#4646](https://github.com/translate/pootle/pull/4646) and
  [#4650](https://github.com/translate/pootle/pull/4650)).

### Triaging

#### Assigned to 2.8

* The editor should be able to handle amaGama error responses better
  ([#4759](https://github.com/translate/pootle/issues/4759)).
* Docs for serializers will be taken care of once there's some stabilization
  towards 2.8 ([#4723](https://github.com/translate/pootle/issues/4723)).
* It needs to be clarified what to do when it comes to displaying stats for
  empty files ([#4748](https://github.com/translate/pootle/issues/4748)).

#### Pushed for the next cycle

* Removing the dependency on Backbone.js is a nice-to-have goal but not a
  priority one ([#4662](https://github.com/translate/pootle/issues/4662)).
  * [Julen](https://github.com/julen) mentioned he has some work done for
    removing Backbone in from the user profile view but will only polish and
    finish it once 2.8 is out
    ([#4663](https://github.com/translate/pootle/issues/4663)).
* There needs to be some review to check if we need more tests for
  `Store.update` when no source/target changes happen
  ([#4715](https://github.com/translate/pootle/issues/4715)).
* Integrating invoices will be taken care of once 2.8 is out.
  [Julen](https://github.com/julen) suggested to follow-up the conversation in
  the issue
  ([#4619](https://github.com/translate/pootle/issues/4715)).
* It would be a desirable enhancement being able to search **and** filter in the
  editor ([#4757](https://github.com/translate/pootle/issues/4757)).
* LDAP support seems low-hanging-fruit, although not a priority one for the time
  being ([#3337](https://github.com/translate/pootle/issues/3337)).

### Future thoughts

#### View mode

* [Ryan](https://github.com/phlax) and [Dwayne](https://github.com/dwaynebailey)
  have been talking about having a sort of _view mode_ in the editor which would
  allow quick string reviews.
* This would have infinite scroll and a lightweight version of the editor, with
  no extra help such as TM matches.
* [Julen](https://github.com/julen) pointed to the export view, and asked
  whether having a editing view as a popup would help.
* There were some quick talks about infinite scrolling in the past, even an
  issue already on track
  ([#3029](https://github.com/translate/pootle/issues/3029)).

#### Customizing the editing widget

* There's some interest for being able to customize the editor's editing widget.
* [Julen](https://github.com/julen) shared a [link to the Plurr live preview
  feature](http://translate.evernote.com/unit/5093147/) used by Evernote in
  production, which is 100% custom code.
* Any customization would definitely require dealing with JavaScript code, as
  there are more interactions and we are relying less and less in templates.

### Next triage meeting

Wednesday 1st of June, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/1).

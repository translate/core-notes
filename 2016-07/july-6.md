## July 6

### Attendees

* [Julen](https://github.com/julen) (Evernote)
* [Leandro](https://github.com/unho) (Translate House)
* [Ryan](https://github.com/phlax) (Translate House)
* [Taras](https://github.com/ta2-1) (Translate House)


### Short status and upcoming endeavours report

* 2.8.0b1 was released. The final 2.8.0 will happen before end of July 2016.
  Bits of `pootle_fs` still need to be landed for that to happen, but it is
  mostly done.


#### Branching and stability

* [Julen](https://github.com/julen) raised the topic of branching and the state
  of current `master`, as `master` has already been branched as `stable/2.8.0`
* Does this mean everything from `master` will be cherry-picked to the stable
  branch?
* Does this mean other code that won't be part of the 2.8.0 release can already
  be merged into `master`?
* There doesn't seem to be consensus on what the `stable/2.8.0` branch even
  means.
* [Ryan](https://github.com/phlax) raised that this can be really confusing for
  anyone checking out the repository, because 2.8.0 hasn't been released yet
  and cannot be considered stable.
* This has been the practice till now (imitating Django's own release process),
  but it's probably time to revisit and clarify how branching will work towards
  releases.


### Triaging

Some new issues this week.


#### Assigned to 2.8

* "Go to string number" fails to set URL properly
  ([#4858](https://github.com/translate/pootle/issues/4870)).


#### Pushed for the next cycle

* Create new project requires "backend" access
  ([#4869](https://github.com/translate/pootle/issues/4869)).
* Stats: create a mechanism to detect if stats are broken
  ([#4863](https://github.com/translate/pootle/issues/4863)).
  * This would help to provide better reporting mechanisms for administrators.
* Translating last unit says "congratulations" regardless of whether task is
  actually finished ([#4795](https://github.com/translate/pootle/issues/4795)).
  * The proper fix is not straightforward, as the client side of the editor
    would need to be aware of statistics.
  * A workaround would be to query the server for stats when performing a
    submission from within the last unit in the result set.


#### Reviewed PRs

The attendees performed a quick review for the open PRs, to share progress and
find out PRs that could be closed. Several PRs where closed.


##### Dirty stats banner

* It's been a bit difficult to find consensus on the matter of disabling the
  dirty stats banner for everyone.
* There's a new PR to disable auto-refresh when there are dirty stats
  ([#4871](https://github.com/translate/pootle/pull/4871)), which diverges from
  the previously-proposed implementation while being non-intrusive for users.
* While stats remain dirty, by default two fetches will be silently performed
  in the background before displaying an informative banner. The wording is
  different for regular users and admins, and there's no ticker displayed
  whatsoever.
* [Taras](https://github.com/ta2-1) will close the old one
  ([#4862](https://github.com/translate/pootle/pull/4862)) once this work has
  been merged.


### Next triage meeting

Wednesday 13th of July, 12 UTC.

----

Please feel free to discuss these notes in the 
[corresponding PR](https://github.com/translate/core-notes/pull/6).

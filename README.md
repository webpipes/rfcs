# Webpipes RFCs

Many changes, including bug fixes and documentation improvements can be
implemented and reviewed via the normal GitHub pull request workflow.

Some changes though are "substantial", and we ask that these be put through a
bit of a design process and produce a consensus among the Webpipes core team.

The "RFC" (request for comments) process is intended to provide a consistent and
controlled path for new features to enter the project.

[Active RFC List](https://github.com/webpipes/rfcs/pulls)

Webpiipes is still **actively developing** this process, and it will still
change as more features are implemented and the community settles on specific
approaches to feature development.

## When to follow this process

You should consider using this process if you intend to make "substantial"
changes to Webpipes or its documentation. Some examples that would benefit from an
RFC are:

- A new feature that creates new API surface area, and would require a feature
  flag if introduced.
- The removal of features that already shipped as part of the release channel.
- The introduction of new idiomatic usage or conventions, even if they do not
  include code changes to Webpipes itself.

The RFC process is a great opportunity to get more eyeballs on your proposal
before it becomes a part of a released version of Webpipes. Quite often, even
proposals that seem "obvious" can be significantly improved once a wider group
of interested people have a chance to weigh in.

The RFC process can also be helpful to encourage discussions about a proposed
feature as it is being designed, and incorporate important constraints into the
design while it's easier to change, before the design has been fully
implemented.

## What the process is

In short, to get a major feature added to Webpipes, one usually first gets the
RFC merged into the RFC repo as a markdown file. At that point, the RFC is
'active' and may be implemented with the goal of eventual inclusion into the
specification.

- Fork the RFC repo http://github.com/webpipes/rfcs
- Copy `0000-template.md` to `text/0000-my-feature.md` (where 'my-feature' is
  descriptive. Don't assign an RFC number yet).
- Fill in the RFC. Put care into the details: **RFCs that do not present
  convincing motivation, demonstrate an understanding of the impact of the
  design, or are disingenuous about the drawbacks or alternatives tend to be
  poorly-received**.
- Submit a pull request. As a pull request the RFC will receive design feedback
  from the larger community, and the author should be prepared to revise it in
  response.
- Build consensus and integrate feedback. RFCs that have broad support are much
  more likely to make progress than those that don't receive any comments.
- Eventually, the team will decide whether the RFC is a candidate for inclusion
  in Webpipes.
- RFCs that are candidates for inclusion in Webpipes will enter a "final comment
  period" lasting 3 calendar days. The beginning of this period will be signaled
  with a comment and tag on the RFCs pull request.
- An RFC can be modified based upon feedback from the team and community.
  Significant modifications may trigger a new final comment period.
- An RFC may be rejected by the team after the public discussion has settled and
  comments have been made summarizing the rationale for rejection. A member of
  the team should then close the RFCs associated pull request.
- An RFC may be accepted at the close of its final comment period. A team member
  will merge the RFCs associated pull request, at which point the RFC will
  become 'active'.

## The RFC life-cycle

Once an RFC becomes active, then authors may submit a finished implementation of
it as a pull request to the Webpipes repo. Becoming 'active' is not a rubber
stamp, and in particular still does not mean the feature will ultimately be
merged; it does mean that the core team has agreed to it in principle and are
amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is 'active' implies
nothing about what priority is assigned to its implementation, nor whether
anybody is currently working on it.

Modifications to active RFCs can be done in followup PRs. We strive to write
each RFC in a manner that it will reflect the final design of the feature; but
the nature of the process means that we cannot expect every merged RFC to
actually reflect what the end result will be at the time of the next major
release; therefore we try to keep each RFC document somewhat in sync with the
language feature as planned, tracking such changes via followup pull requests to
the document.

## Implementing an RFC

The author of an RFC is not obligated to implement it. Of course, the RFC author
(like any other developer) is welcome to post an implementation for review after
the RFC has been accepted.

If you are interested in working on the implementation for an 'active' RFC, but
cannot determine if someone else is already working on it, feel free to ask
(e.g. by leaving a comment on the associated issue).

## Reviewing RFCs

Each week the team will attempt to review some set of open RFC pull requests.

We try to make sure that any RFC that we accept is accepted at the weekly team
meeting. Every accepted feature should have a core team champion, who will
represent the feature and its progress.

**THe Webpipes RFC process owes its inspiration to the [Gatsby RFC process],
[React RFC process], [Yarn RFC process], [Rust RFC process], and [Ember RFC
process]**

[gatsby rfc process]: https://github.com/gatsby/rfcs
[react rfc process]: https://github.com/reactjs/rfcs
[yarn rfc process]: https://github.com/yarnpkg/rfcs
[rust rfc process]: https://github.com/rust-lang/rfcs
[ember rfc process]: https://github.com/emberjs/rfcs

# Requirements for Open Development communications channels

**tl:dr; Contributions to this (public) list of requirements are welcome, using this repository's issue tracker for discussion**

In Apache projects we say

> If it didn't happen on the dev list, it didn't happen

Meaning that all important technical discussions and decisions about the project _must_ happen on a central shared channel to enable efficient collaboration in globally distributed teams.

Mailing lists have served us well in the last few decades but they can also be rightly considered an old and clunky tool.

However, to this day, I haven't seen a better tool for the types of long-lived and complicated discussions that lead to creating great software.

Newer tools (like Slack in particular, which is trendy these days) are much more convenient and fun to use, but I think they lack support for some of our more complex communications use cases.

After arguing many times with colleagues (both at work and in Apache projects) about which tool is best, I think it is useful to forget about the tools for a while, and concentrate on the _collaboration use cases_ that we want to enable.

So here we go - I'll start with a few draft use cases below and we can use the issue tracker of this repository to get contributions from anyone who wants to join this discussion.

If you're interested, my reading list at https://pinboard.in/u:bdelacretaz/t:opendevelopment/ has more information on Open Development, as seen by a long-term Apache community member.

I have also written a [Large Mailing Lists Survival Guide](http://blogs.adobe.com/opendev/2014/05/28/large-mailing-lists-survival-guide/) with best practices that are more specific to mailing lists.

## Building Blocks

Let's try to define basic requirements as building blocks that the use cases that follow can refer to.

* *Just Talk* : exchange message with others with reasonable assurance that they can read and reply to them
* *Precise Quoting*: be able to indicate very precisely which part of the previous message you are replying to.
* *Join Later*: be able to join a discussion efficiently much later than it started, without losing context
* *Ignore The Rest*: efficiently mute the parts of the overall conversation that are not relevant to you
* *Split Thread*: split a discussion into several clearly identified subtopics
* *Voting*: present a set of options and allow people to rank them
* *Formal Audit*: be able to find and retrieve any discussion thread in its entirety, forever
* *Categorize Content*: be able to mark existing messages based on their topics, quality, relevance etc.

## Open Development Communications Channels Use Cases

**All this is a DRAFT for now** - feel free to discuss using this repository's issue tracker, referring to the use cases IDs.

## Quick throwaway discussion
_Scenario_: Discuss something that won't stay relevant for long, and can be safely ignored by whoever's not present when the discussion happens.

_Example_: "Does anyone want to join for dinner at Bob's Snails Place today"

_Challenges_: None

_Requirements_: Just Talk

## Technical Q&A
_Scenario_: Someone asks a question, several people potentially provide answers of various quality.

_Challenges_: Provide a way to mark the best answers, make it easy to find and refer to previous answers

_Requirements_: Just Talk, Join Later, Categorize Content

## Discussing a complex technical problem
_Scenario_:  Describe a complex technical problem and explore possible solutions

_Challenges_: 
The discussion can last for a long time and people need thinking time, so there might be large gaps during which nothing happens, and the discussion picks up again later.

People might be absent when the discussion starts but might have relevant input later. They need to be able to review and join the discussion efficiently at any time.

In a long-lived project, such complex discussions can reoccur regularly, in which case it must be easy to point people to the prior occurences.

_Requirements_: Just Talk, Precise Quoting, Join Later

## Discussion that forks into a tree
_Scenario_: A discussion that started a while ago needs to be split into several subtopics, without losing context and history for any of them. Each subtopic might be a complex discussion.

_Challenges_: Each subtopic needs to be clearly identified and segregated, to allow people from ignoring the subtopics that are not relevant to them.

_Requirements_: Just Talk, Precise Quoting, Join Later, Split Thread, Ignore The Rest

## Polling the community and/or voting
_Scenario_:  Present a set of options to the community and let people express their preferences

_Challenges_: For a poll, need reasonable assurance that people will have seen the poll, even if they were absent when it was sent. For a formal vote, might need a formal way for people to confirm that they have seen it.

_Requirements_: Voting, Formal Audit

# Requirements for Open Development communications channels

**tl:dr; Contributions to this (public) list of requirements are welcome, using this repository's issue tracker for discussion**

In Apache projects we say _if it didn't happen on the dev list, it didn't happen_ meaning that all important technical discussions and decisions about the project _must_ happen on a central shared channel to enable efficient collaboration in globally distributed teams.

Mailing lists have served us well in the last few decades but they can also be rightly considered an old and clunky tool.

However, to this day, I haven't seen a better tool for the types of long-lived and complicated discussions that lead to creating great software.

Newer tools (like Slack in particular, which is trendy these days) are much more convenient and fun to use, but I think they lack support for some of our more complex communications use cases, especially for the types of chaotically distributed teams that are the norm in many open source projects.

Mailing lists can also be very inefficient if used the wrong way, with sloppy quoting, vague subject lines and multiple topics per thread. The [Large Mailing Lists Survival Guide](https://grep.codeconsult.ch/2017/11/10/large-mailing-lists-survival-guide/) that I wrote for our Adobe open development blog lists best practices for using them, and shows that you need lots of discipline for them to work well.

After arguing many times with colleagues (both at work and in Apache projects) about which tool is best, I think it is useful to forget about the tools for a while, and concentrate on the _collaboration use cases_ that we want to enable.

So here we go - I'll start with a few draft use cases below and we can use the issue tracker of this repository to get contributions from anyone who wants to join this discussion.

If you're interested, my reading list at https://pinboard.in/u:bdelacretaz/t:opendevelopment/ has more information on Open Development, as seen by a long-term Apache community member.

## Credits
All contributions will be duly credited here, of course.

## Building Blocks
Let's try to define basic requirements as building blocks that the use cases that follow can refer to.

* *Just Talk* : exchange message with others with reasonable assurance that they can read and reply to them
* *Precise Quoting*: be able to indicate very precisely which part of the previous message you are replying to. Also known as [Usenet Quoting](https://en.wikipedia.org/wiki/Usenet_quoting) in email.
* *Join Later*: be able to join a discussion efficiently much later than it started, without losing context
* *Ignore The Rest*: efficiently mute the parts of the overall conversation that are not relevant to you
* *Split The Thread*: split a discussion into several clearly identified subtopics
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

## Questions and Answers
_Scenario_: Someone asks a question, several people potentially provide answers of various quality.

_Challenges_: Provide a way to mark the best answers, make it easy to find and refer to previous answers

_Requirements_: Just Talk, Join Later, Categorize Content

## Brainstorming a complex technical topic
_Scenario_:  Describe a complex technical topic and explore possible solutions

_Challenges_: 
The discussion can last for a long time and people need thinking time, so there might be large gaps during which nothing happens, and the discussion picks up again later.

People might be absent when the discussion starts but might have relevant input later. They need to be able to review and join the discussion efficiently at any time.

In a long-lived project, such complex discussions can reoccur regularly, in which case it must be easy to point people to the prior occurences.

_Requirements_: Just Talk, Precise Quoting, Join Later

## Building Consensus
_Scenario_ : Once the brainstorming and options definitions are over, move forward with consensus building. 

_Challenges_: 
The discussion can last for a some time, people might be absent during part of it but need to be able to review and join the discussion efficiently at any time.

The consensus building discussion needs to be archived and easy to find later, as it is the core of the decision making process. A lack of indexed archives might lead to having to explain things again later.

_Requirements_: Just Talk, Precise Quoting, Join Later, Formal Audit

## Making a Decision
_Scenario_ : Once the consensus building phase is over, make a decision either from an obvious consensus or by voting if needed.

_Challenges_: 
This phase needs to be archived and easy to find later, like the consensus building phase, for the same reasons and also to have a formal trace of the decision.

_Requirements_: Just Talk, Precise Quoting, Join Later, Voting, Formal Audit


## Discussion that forks into a tree
_Scenario_: A discussion that started a while ago needs to be split into several subtopics, without losing context and history for any of them. Each subtopic might be a complex discussion.

_Challenges_: Each subtopic needs to be clearly identified and segregated, to allow people from ignoring the subtopics that are not relevant to them.

_Requirements_: Just Talk, Precise Quoting, Join Later, Split The Thread, Ignore The Rest

## Polling the community and/or voting
_Scenario_:  Present a set of options to the community and let people express their preferences

_Challenges_: For a poll, need reasonable assurance that people will have seen the poll, even if they were absent when it was sent. For a formal vote, might need a formal way for people to confirm that they have seen it.

_Requirements_: Voting, Formal Audit

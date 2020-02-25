# Conversation with VV

## Twitter DMs

VV: If Whitehead is groundbreaking, albeit 100+ yo, resurfacing it may be like finding the treasures in the Titanic and bringing them back to civilization. However, if that can be done it must be by means of simple words, not going beyond the 70th percentile, or even less.

John: I do think Whitehead's Process and Reality is a challenging book to read in its entirety. However, I do think his "categories of existence" should be recognizable for anyone who has experienced event sourcing or event storming. Apparently he started his lectures, which he gave for two years before publishing his book, by listing out his categories. In a high pitched voice. Not sure why high pitch, perhaps he was a bit nervous about it.

The first category is "actual occasions" which corresponds to "domain event". The second is "prehensions" or "feelings", which are facts of relations of one actual occasion to others. The third is " nexus" which he also called "event" is just a set of actual occasions, and corresponds to the domain events of an aggregate (nexus with serial or "personal" order) or of an application (nexus with non-personal social order) or of a random bunch of occasions (non-social nexus, or chaos). There are eight such categories, but I think they are perfectly recognizable. That's the "hard core" of it, anyway.


VV: Why does it matter? Is it groundbreaking in any way?

John: Well, the question I had, a few years ago after doing event sourcing for a little while, for which I was looking for a good answer, was: how general is this consideration of the events in a domain? what does it overlook, and is it exhaustive of the actual concerns? are there any domains which would evade such a consideration, or when will it let you down?

Whitehead said (in a letter to Bertrand Russell, who was badgering Whitehead for his notes before he had published Process and Reality, when Russell complained to Whitehead that Russell couldn't work without Whitehead's notes) that he had been working on this stuff his whole life. It's said Whitehead read the Greeks (Plato, Aristotle, etc) in Greek when he was a boy. He read all the other major figures, and found the whole thing rather incoherent. He effectively refactored Western philosophy. So we can look at what he did from that point of view.

In my understanding, he did two critical things. He accepted the "atomism" of the Greeks, but instead of the "atoms" being instances of the substance-quality categories, he took the idea from Locke that the actual entities are actual occasions of experience. He rejects the mind-body duality of Descartes in his speculating that all actual entities have a mental and physical pole, with conscious intellectuality being a high grade of mentality. He said his actual occasions are like the monads of Leibniz's Monadology, but with the modification that Whitehead's monads (the "actual occasions") don't change. That seems aligned with the design of our "immutable domain event" proposed as "first class citizens".

It seems to me that, through the empirical reality of making software systems actually work, we (or perhaps it was just Greg Young) came to the exactly the same conclusion in the 2000s as Whitehead did in the 1920s. The difference is that Whitehead's "new system" is an actual cosmology, and his stated claim is that "the scheme should have developed all those generic notions adequate for the expression of any possible interconnection of things". Whereas event sourcing is a design that can be used in a software system. The "immutable domain event" is a special case of Whitehead's notion of an actual occasion, and we can consider everything else from this point of view (hence the name "categories of existence").

So, for example, you can look at "agile" and ask to what extent it avoids the substance-quality categories, and the answer is "not very well" since "agile" is the quality that the team "substance" should have, and people ask whether any given team is or is not "agile". You can also appreciate more things like Scrum which define particular events (the scrum events). EPISODES stands out as feeling much of what Whitehead felt ("we find facts, share opinions, build concentration and generally prepare for an event that cannot be known in advance. After the climax, the decision...").

And pattern language seems like a direct application of Whitehead's system, and it turns out that Alexander was at Harvard a few decades after Whitehead, so this stuff would probably have been in the air, and anyway he cites Whitehead, and much of the "mysteriousness" of Timeless Way of Building is just a poetic rendering, for architects of the built environment, of Whitehead's scheme. Ward Cunningham, I feel, was sensitive enough to feel what Whitehead was saying reflected in the work of Christopher Alexander, and that's why he was able to write EPISODES. But then perhaps Fowler wasn't sensitive enough, and in consequence operates with an inadequate concept of an event (which is why Greg Young was right to criticise Fowler's take on events-as-commands).

It follows from Whitehead's system that you would expect to find everybody feeling what he said to some extent or other, and to the extent that they feel it they make sense, and to the extent that they don't feel it, they don't make sense. People also seem to feel it differently at different times, for example Fowler's refactoring book feels very much like a description of actual occasions, particularly the way a refactoring starts with a code smell, which is basically a set of feelings that suggest a better settlement can be found.

For me, putting the design of software systems to one side for a moment, it's the human process which I think is better conceived and proposed in terms of actual occasions. All the proposals to establish "continuous" anything distract from attending to settling a set of feelings into an actual occasions. That's what TDD is about, and also fixed timeboxes. But really a team is also an event. Whitehead suggested there is no togetherness except in the becoming of an actual occasion. That's why classic "team building" is always terrible, and is always a failure. It's also why mob programming can easily be a "thing". But when relating to others, I find it helps to keep things real to focus on the next step, and the one after that, and remember that's actually quite optimal, since looking for the general principles and the stead state and the continuous process really just subtracts from attending to settling a set of feelings into a single settled unity that is an actual occasion by which our worlds are built up. I think that's a useful thing to know.

This isn't to say that the physical objects we encounter is the world are just illusions. Instead, it allows us to understand that their nature is the result of their history ("nature = history"), rather than "instances of substance-quality categories". Whitehead wrote, "These enduring objects and 'societies' analysable into strands of enduring objects, are the permanent entities which enjoy adventures of change throughout time and space." As you can see, it's perfectly readable, and perfectly recognisable especially for anybody who has experienced event sourcing or event storming for any length of time.

VV: I think the first requirement is a glossary on the terms used, without going down the rabbit trail into a tome on each or recursion.

John: Yes that makes sense. Terms of reference, or ubiquitous language :-)

[a bit later]

Good morning :) I have been thinking about our glossary...

Firstly, I suppose it must include "actual occasion”. I remember what you said about not writing a tome, but I just spent an hour or so writing the following summary:

Whitehead wrote, "The Category of the Ultimate" expresses the general principle presupposed in the three more special categories. 'Creativity', 'many', 'one' are the ultimate notions involved in the meaning of the synonymous terms 'thing', 'being', 'entity'. These three notions complete the Category of the Ultimate and are presupposed in all the more special categories."

"The term 'one' does not stand for 'the integral number one', which is a complex special notion. It stands for the general idea underlying alike the indefinite article 'a' or 'an' and the definite article 'the' and the demonstratives 'this' or 'that' and the relatives 'which' or 'what' or 'how'. It stands for the singularity of an entity."

"The term 'many' presupposes the term 'one' and the term 'one' presupposes the term 'many'. The term 'many' conveys the notion of 'disjunctive diversity'; this notion is an essential element in the concept of 'being'. There are many 'beings' in disjunctive diversity."

"'Creativity' is the universal of universals characterizing ultimate matter of fact. It is that ultimate principle by which the many, which are the universe disjunctively, become the one actual occasion, which is the universe conjunctively. It lies in the nature of things that the many enter into complex unity."
Then onwards to the Categories of Existence...

Copying from Whitehead:

"There are eight Categories of Existence: 

(i) Actual Entities (also termed Actual Occasions), or Final Realities, or Res Verae.

(ii) Prehensions, or Concrete Facts of Relatedness. 

(iii) Nexus (plural of Nexus), or Public Matters of Fact. 

(iv) Subjective Forms, or Private Matters of Fact. 

(v) Eternal Objects, or Pure Potentials for the Specific Determination of Fact, or Forms of Definiteness. 

(vi) Propositions, or Matters of Fact in Potential Determination, or Impure Potentials for the Specific Determination of Matters of Fact, or Theories. 

(vii) Multiplicities, or Pure Disjunctions of Diverse Entities. 

(viii) Contrasts, or Modes of Synthesis of Entities in one Prehension, or Patterned Entities."

I didn't really get very far into the Categories of Explanation yet, and I don't really know what the Categoreal Obligations are. But I think it does make sense to expand on "Nexus" (the third category of existence) because that's what Whitehead refers to when he uses the word "event".

A nexus has actual occasions as "members", so I reckon it's a least a bit like a set. But there are different types, that are characterised by their degree of order. Whitehead says that an actual occasion is the "limiting type" of a nexus with only one member. Obviously there isn't any scope for different orderings of only one thing. A nexus that has one occasion followed by another is an event that is definitely not an actual occasion. Like "dual writes" it isn't atomic in its subjective aim, since there are two of them. Moving on, a nexus either has "social order" or it doesn't. For a nexus to have social order, there must be a "fact of togetherness" shared by the actual occasions that are members of this nexus. With a fact of togetherness, the nexus is a non-social nexus, and Whitehead says this corresponds to the notion of "chaos". If the actual occasions are ordered serially, the "social order" is a "personal order". A social nexus is a society of events, and a society that has many strands of personal order is called a "corpuscular society". The physical enduring objects we encounter is the real world are all societies of events.
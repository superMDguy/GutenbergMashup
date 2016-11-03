# GutenbergMashup

Hopefully good and __interesting__ novel generator for NaNoGenMo 2016

##Original Plan
Last year, there was a discussion about how most novels are boring (see https://github.com/dariusk/NaNoGenMo-2015/issues/11). In response to this, cpressey created "A Time for Destiny: The Illustrious Career of Serenity Starlight Warhammer O'James during her First Three Years in the Space Fighters", using a story compiler approach. However, as he noted, the story is interesting for a bit, but then starts to get less interesting. Why?

I think that anything built using manually created templates inherently has this "boring point". No matter how many templates you write, your novel will eventually have a "boring point", where the novel feels repetitive. You start to sense the templates inside, and see where names where inserted in formulas. One could argue that the only way to defeat this would be to have a human mind behind the story. When you get to the bottom of it, though, I'd say the human mind really is just a collection of "templates", that creativity is merely rearranging these templates in interesting ways. Everything we do is influenced by things we've read and experienced. So, the answer is to create as many templates as the human mind has, or just as many as possible.

Enough with the theory. Here's what I plan to do:

1. Get as many Project Gutenberg books as possible.
2. Analyze the texts, trying to find named entities like "main character", "love interest", "principal setting", "goal (whether an action, state, or object". I'll probably do this using a combination of word counts, relations between objects, and POS tagging using spaCy or NLTK.
3. Create templates based on this analysis, for example inserting {character(main)} wherever "Sherlock Holmes" appears in a Arthur Conan Doyle novel.
4. Break up the novel into 'scenes'. This will be a really hard part. I'll probably start out by just using chapters, and make it more accurate later if I have time.
5. Pick random entities from the list derived from the PG ebooks, and assign them to their entity name, for example choosing "Elizabeth" as the main character.
6. Create a plot with a plot generator.
7. Use the scenes with filled in entities to generate the text for the plot.
8. This might be overambitious (it definitely is), but I'll just see how far I can get. Let's see how this works.

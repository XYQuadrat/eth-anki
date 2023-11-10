# eth-anki

Are you searching for Anki cards for most of the courses in the Computer Science Bachelor at ETH Zurich? Then you came to the right place.
This repository contains over 700 (hopefully) high-quality flashcards for many lectures, and you can easily contribute too!

## How can I import this collection into Anki?

This repository uses the [CrowdAnki](https://github.com/Stvad/CrowdAnki) JSON-based format for interfacing with Anki.
CrowdAnki makes it possible for you to easily update the collection with cards added after the initial import whilst preserving your learning progress, which is hard to do with the normal .apkg format of Anki.

First, install the [CrowdAnki add-on](https://ankiweb.net/shared/info/1788670778) in the desktop version of Anki.

Then, download the latest release of this collection from the [Releases page](https://github.com/XYQuadrat/eth-anki/releases) and extract the archive.

Now go to `File -> CrowdAnki: Import from disk` and choose the directory you extracted the archive into. You should not need to change anything in the _Import Settings_ dialog. After the import finishes, you should now see a "ETH D-INFK" deck in Anki containing all the cards.

## Design Decisions

- I use a single deck for all notes, and then tag each note with the relevant course(s). Tags allow for more flexibility than subdecks, because a note might be relevant for several courses. You can easily study the cards for just one particular course with [filtered decks](https://docs.ankiweb.net/filtered-decks.html). (When I started the collection, the Anki scheduler was only able to introduce new cards in deck order, which was also an argument against using many subdecks.)
- I structure the tags hierarchically by semester. This makes searching for a particular tag easier.
- I believe that good, effective cards mostly follow the [twenty rules of formulating knowledge](https://www.supermemo.com/en/blog/twenty-rules-of-formulating-knowledge). By far not all cards do this right now, but it is the goal that one day they all will.
- I really like cloze deletions (this is partially based on the rules mentioned above).
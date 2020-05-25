# Anki Decks

The anki decks that I maintain.


## Homemade vs "Forked"

I should export any independent deck here, before beginning to use it. This will make it easier to diff my change as I update the deck for my preferences.


## Deck Management

I would eventually like to write a deck generator for some common structured data types.

In the meantime, I am going to write some decks by hand to understand the complex features in detail.

Remember that cards are descendants of notes. Notes are abstract between decks, your entire account is called a "collection" of notes.

I am not sure how attached media works. Some Nederlands language cards have attached sound files, and I would like to attach my own to practice punctuation.


## Backup Considerations

Backup often; as possible.

The subdeck struture is probably preserved in the `.apkg`. The cards and notes do not preserve much structure. I think one of them preserves tags.

- Anki server is free software and can sometimes fail to reconcile and import or export
- It also doesn't track history very well


## Backup Process

Use the macos anki application installed by `brew cask install anki`.

We want to backup the deck binary export, the notes, and the cards.

1. Export your deck and subdecks as a "Anki Deck Package" or `.apkg` file by selecting the main deck parent.
  - This is a binary package
2. Export your deck and subdecks as "Notes in plain text". Use the same filename as the previous export. 
  - This is easy to diff visually
  - This is roughly a TSV file, so it might be usable later
2. Export your deck and subdecks as "Cards in plain text". Use the same filename as the previous export. 
  - This is easy to diff visually
  - This is roughly a TSV file, so it might be usable later

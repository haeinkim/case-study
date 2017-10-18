# OOP - Case study I
This is a simple command-line notebook application. 

## Goal of this project
Getting some idea in common usage of classes, functions, methods, and docstrings.

## Examples
### Using Notebook module directly
    >>> from notebook import Note, Notebook
    >>> n = Notebook()
    >>> n.new_note("hello world")
    >>> n.new_note("hello again")
    >>> n.notes
    [<notebook.Note object at 0xb730a78c>, <notebook.Note object at
    0xb73103ac>]
    >>> n.notes[0].id
    1
    >>> n.notes[1].id
    2
    >>> n.notes[0].memo
    'hello world'
    >>> n.search("hello")
    [<notebook.Note object at 0xb730a78c>, <notebook.Note object at
    0xb73103ac>]
    >>> n.search("world")
    [<notebook.Note object at 0xb730a78c>]
    >>> n.modify_memo(1, "hi world")
    >>> n.notes[0].memo
    'hi world'
### Using Menu interface

1. You don't have any note at the first time. So, just enter "3" to select "Add Note"
2. Type some note. Making a list of notes for experiment.
3. To confirm your note list, type "1" and it will print out the list.
4. You can modify specific memo through the "4"
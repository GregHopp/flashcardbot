# flashcardbot
# This is a tool to create a spreadsheet (ultimately to used for flashcards)
# while reading an Arabic text. It first requests a sheet name, and creates
# and saves a sheet under that name, with marked Arabic and English columns.
# It uses a counter to track what row a given term is on. It operates on a
# while loop, saving the sheet andasking the user for a term with each
# iteration. Normally, the user will input an Arabic term, the program will
# present the translation, and the user will accept by hitting enter. This
# saves the term and the translation to the sheet. The user can also input
# their own translation.

# When a translation is presented, the user can also type "hold" or "skip"
# (this can be done even if the keyboard in set to Arabic, by pressing the
# same keys as you would in English).

# "Hold" adds the term to a list of held terms, but does not enter it in the
# sheet. Unless the user comes back to it, there will be no trace of it at the
# end. This is most useful for when the user is unsure if the term is important,
# and prevents the creation of cards with blank translations. If the term is
# later reentered and a translation given, it will be appended to the bottom of
# the table like any other term.

# "Skip" adds the term to a list of skipped terms, as well as to the sheet. This
# is most useful when the creation of flashcards from the sheet is not automated,
# or where the term is important but will require further research to determine
# an appropriate meaning. If the term is later reentered and a translation given,
# it will appear where it would have if it was not skipped.

# "Show" will produce the held and skipped lists, and once again present the
# translation for acceptance. "Show" can also be used when asked for a term.

# When asked for a term, the user has the option of typing "phrase." This is
# useful for when a whole clause or sentence must be translated in order to
# clarify its meaning. The user has three options, they can accept the given
# translation, they can enter their own, or they can skip. The phrase and its
# translation (or just the phrase, if skipped), are entered D and E columns,
# respectively.

# If the user types 'done' when asked for a term, they are first presented with
# the current skipped and held terms. They can end the program by hitting
# "enter," or they can cancel by typing any character and hitting "enter."

# When the program is ended, it saves the workbook, and informs the user.

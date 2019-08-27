# Aspell Personal Dictionaries

## Usage for Spanish analysis

1. Download the word_list file.

        wget -O spanish_word_list https://raw.githubusercontent.com/jnonino/aspell-personal-dictionaries/master/spanish_word_list
    
2. Generate the Aspell dictionary for Spanish adding the word list.

        aspell --lang=es create master ./list.pws < spanish_word_list
    
3. Move the recently created dictionary to the Aspell folder.

        mv list.pws /usr/lib/aspell/
    
4. Add the dictionary to the spanish checks

        echo "add list.pws" >> /usr/lib/aspell/es.multi

5. Use the Aspell command as usual

        aspell --lang=es

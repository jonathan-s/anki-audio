
# Install

```
# ensure that you run python 3.11
pip install uv

# if you have higher version of python, you can create a venv with python 11
uv venv -p 3.11
source .venv/bin/activate

# doing pip install takes ages.
uv pip install tts  
```

Generate audio
- Copy collection.anki2 into the directory
- `python generate_audio.py`

```shell
ln -s path-to-anki-directory anki_dir
# directory is something like ~/Library/Application\ Support/Anki2/User\ 1 on mac
```

Output to mp3
```shell
sox output2.wav -C 128 output.mp3
```

## Speakers

dict_keys(
    ['Claribel Dervla', 'Daisy Studious', 'Gracie Wise', 'Tammie Ema', 'Alison Dietlinde', 'Ana Florence', 'Annmarie Nele', 'Asya Anara', 'Brenda Stern', 'Gitta Nikolina', 'Henriette Usha', 'Sofia Hellen', 'Tammy Grit', 'Tanja Adelina', 'Vjollca Johnnie', 'Andrew Chipper', 'Badr Odhiambo', 'Dionisio Schuyler', 'Royston Min', 'Viktor Eka', 'Abrahan Mack', 'Adde Michal', 'Baldur Sanjin', 'Craig Gutsy', 'Damien Black', 'Gilberto Mathias', 'Ilkin Urbano', 'Kazuhiko Atallah', 'Ludvig Milivoj', 'Suad Qasim', 'Torcull Diarmuid', 'Viktor Menelaos', 'Zacharie Aimilios', 'Nova Hogarth', 'Maja Ruoho', 'Uta Obando', 'Lidiya Szekeres', 'Chandra MacFarland', 'Szofi Granger', 'Camilla Holmström', 'Lilya Stainthorpe', 'Zofija Kendrick', 'Narelle Moon', 'Barbora MacLean', 'Alexandra Hisakawa', 'Alma María', 'Rosemary Okafor', 'Ige Behringer', 'Filip Traverse', 'Damjan Chapman', 'Wulf Carlevaro', 'Aaron Dreschner', 'Kumar Dahl', 'Eugenio Mataracı', 'Ferran Simen', 'Xavier Hayasaka', 'Luis Moray', 'Marcos Rudaski'])


## Other tts
```
# Install tts
brew install tts

# List available models
tts --list_models

# Generate a sample
tts --text "Um. Es geht um einen Mann namens Carsten Martens." \
--model_name "tts_models/de/thorsten/vits" \
--out_path ./um.wav
```

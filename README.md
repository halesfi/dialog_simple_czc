# Dialog for Pepper to switch between languages

Developed at [NLP Centre](https://nlp.fi.muni.cz/en), [FI MU](https://www.fi.muni.cz/index.html.en) for [Karel Pepper](https://nlp.fi.muni.cz/trac/pepper)

The application is to be installed from the `dialog_simple_czc-0.1.2.pkg` file.

The application contains two simple dialogs - English and Czech ones. Czech is an example of a "partly supported" language at the Pepper robot - it can be used for ASR and TTS, but the system applications do not (yet) contain Czech dialogs.

This application allows to start creating new dialogs in Czech and to ask Pepper to use them by switching to Czech when talking.

# Example dialog

Pepper is in English by default.
* **User**: *Pepper Speak Czech* - this command usually does not work, as the same command is covered by the system dialogues, which say that there are no dialogs for Czech available. This was solved by the following workaround.
* **User**: *Mluv česky* - this is actually the Czech equivalent for "Speak Czech". The English ASR engine contains this command in the "phonetic" form as *mloof cheski* and it works :simple_smile:
* **Pepper**: *Let's speak Czech!*
* **Pepper**: *Teď mluvím česky.* (eq. *Now I speak Czech*)
* **User**: *Ahoj* (eq. *Hello*)
* **Pepper**: *Ahoj*
* **User**: *Jak se máš?* (eq. *How are you?*)
* **Pepper**: *Já se mám suprově.* (eq. *I feel super*)
* **User**: *Mluv anglicky* (eq. *Speak English*)
* **Pepper**: *Dobře, budu mluvit anglicky!* (eq. *Ok, I will speak English!*)
* **Pepper**: *Now I speak English*

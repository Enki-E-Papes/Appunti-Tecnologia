# ***Comandi Git***

fai il commit delle tue modifiche sul repository locale.

    - git add *
    - git commit -m "commit_uno"

creazione del branch:

    - git checkout -b "feature_X"

    (dove X è il numero con cui inizia il nome della tua cartella).[In realtà questa sintassi è equivalente a:]
	git branch "feature_X"
	git checkout "feature_X"
****
fare modifiche .
****
ritorna sul branch principale:

    - git checkout main
    - git push origin "feature_X"

 puoi vedere l'elenco dei branch con questo comando:

    - git branch

 puoi vedere l'elenco di tutti i branch (sia del repository locale che di quello remoto) con questo comando:

	- git branch -a

ritorna nel branch principale:

	- git checkout main

lancia il comando:

	- git branch -d <nome del branch>

*ELIMINARE UN BRANCH DEL REPOSITORY REMOTO*

puoi eliminare un branch del repository remoto con questo comando:
	git push origin -d feature_X (dove feature_X è il nome del tuo branch)

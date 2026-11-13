# Part 1: Bones pràctiques en la documentació de commits

## Crear el README
![Captura_creacio_README](img/readme.png)

## Commit "docs: inicialitza la repositori de prova per tasca 2"
![Commit_Inici_tasca02](img/commit.png)

## Crear el fitxer 00-installer-config.yaml
![Creacio_fitxer_00-installer-config.yaml](img/00-installer-config.png)


# Part 2: L'historial del repositori

## Observa l'historial del teu repositori amb l'historial detallat, identificant la informació disponible per cada commit
![captura_git-log](img/git-log.png)

## Compara el resultat amb l'historial resumit
![captura_git-log--oneline](img/git-log--oneline.png)

## Usa l'eina gràfica de l'editor VS Code per veure l'historial del repositori i comparar-lo amb el que has vist a la terminal
![captura_git-graph](img/git-graph.png)

## Inspecciona els canvis exactes del darrer commit
![captura_git-show-HEAD](img/git-show-HEAD.png)

## Observa també la mateixa informació amb l'eina gràfica de l'editor VS Code, seleccionant el darrer commit.
![captura_git-graph_HEAD](img/HEAD-git-graph.png)


# Part 3: Recuperar versions anteriors del working directory

## Simularem un error humà editant el fitxer 00-installer-config.yaml
![captura_editar-00-installer-config.yaml](img/editar_00-installer-config.png)

## Observa l'estat del repositori. A l'editor VS Code, veuràs que el fitxer interficies.yaml apareix amb una M, indicant que ha estat modificat.
![M](img/m.png)

## A la terminal, executa la comanda al terminal per comprovar com t'indica aquesta situació
![captura_M_status](img/M-status.png)

## Desfem els canvis del fitxer interficies.yaml i tornem-lo a l'estat del darrer commit. Això es pot fer gràficament a l'editor VS Code, fent clic amb el botó dret sobre el fitxer i seleccionant l'opció "Discard changes". També es pot fer des de la terminal amb la comanda
![captura_discard_changes](img/discard-changes.png)

## Pots comprovar que l'estat del repositori és correcte amb la comanda git status
![captura_status_dc](img/git-status-DC.png)

# Part 4: Recuperar versions anteriors (commits) del repositori

## Editarem l'arxiu 00-installer-config.yaml i modificarem el valor de dhcp4 a false i afegirem una un configuració estàtica a la interfície enps03
![captura_dhcp4_enps03](img/dhcp4-enps03.png)

## Editem de nou l'arxiu, ara per configurar una segona interfície enps08 en mode DHCP
![captura_enps08_DHCP](img/enps08-DHCP.png)

## Per últim, incorporem canviem els servidor DNS a la configuració de la interfície enps03, perquè la configuració inicial no funcionava correctament
![captura_DNS_enps03](img/DNS-enps03.png)

## Revisa ara l'historial del repositori amb la comanda git log --oneline o amb l'eina gràfica per veure tot l'historial de commits realitzats
![captura_oneline_part4](img/oneline-part4.png)

## Anem a documentar un exemple de revert d'un commit
![captura_revert](img/revert.png)

## Explorar un commit anterior
![captura_4_commit](img/4-commit.png)

## Finalment, tot i que no és un procediment recomanat, anem a eliminar el darrer commit (git reset)
- Mostra l'historial actual amb la comanda git log --oneline
![captura_oneline4](img/oneline.png)
- Elimina el darrer commit bé sigui amb la comanda git reset --hard HEAD~1 o amb l'eina gràfica
![captura_git_reset](img/git-reset.png)
- Indica l'estat del repositori amb la comanda git status i mostra l'historial amb la comanda git log --oneline
![captura_git_status4](img/git-status4.png)
![captura_oneline_final](img/oneline-final.png)
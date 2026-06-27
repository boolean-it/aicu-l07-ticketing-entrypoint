# Consegna - Lezione 07

## Obiettivo

Preparare il brief tecnico del lab L08 senza avviare ancora la patch.

Task:

```txt
Serve creare ticket dal supporto.
```

Come visto in aula, devi localizzare dove potrebbe entrare la modifica, leggere evidenze minime nel repo e preparare il prompt patch limitato che userai nel lab.

## Prima Di Compilare

Oggi userai tre artefatti:

| Artefatto | Che cos'e' | A cosa serve | Output atteso | Errore tipico |
| --- | --- | --- | --- | --- |
| Mappa dei punti di intervento (entry-point map) | Mappa dei file o aree verificati | Separare ipotesi AI da evidenza nel repo | File ammessi, dubbi e vietati con motivo | Segnare come ammesso un file non letto |
| Prompt patch limitato | Prompt per il primo slice del lab | Dire al builder cosa fare e dove fermarsi | Task, file, fuori scope, verifica, stop condition | Chiedere una feature completa |
| Reviewer leggero | Prompt/checklist di controllo | Far controllare file, contract, diff e verifica | Findings, verifiche mancanti, decisione | Chiedere nuove idee o redesign |

Come visto in aula: una proposta AI non e' una prova. Prima leggi il repo, poi decidi cosa autorizzare.

## Repository Di Lavoro

Lavora nel tuo fork della repo:

```txt
aicu-m02-l07-ticketing-entrypoint
```

Prima di iniziare, importa solo questi artefatti:

```txt
aicu-m02-l05-ticketing-issue/output/issue-create-ticket.md
  -> lavoro-precedente/issue-create-ticket.md

aicu-m02-l06-ticketing-contract/output/contract-sketch-create-ticket.md
  -> lavoro-precedente/contract-sketch-create-ticket.md

aicu-m02-l06-ticketing-contract/output/data-sketch-create-ticket.md
  -> lavoro-precedente/data-sketch-create-ticket.md
```

Non copiare le repo precedenti intere.

## Input

Usa:

```txt
template/entry-point-map.md
template/prompt-patch-limitato.md
template/reviewer-leggero.md
```

Porta con te:

- issue L05;
- contract sketch L06;
- data sketch L06.

## Passaggi Per Risolvere L'Esercizio

Segui questi passaggi in ordine. L'obiettivo non e' scrivere codice: l'obiettivo e' preparare il pacchetto che userai nel Lab08.

1. Importa solo questi output in `lavoro-precedente/`:
   - `issue-create-ticket.md`;
   - `contract-sketch-create-ticket.md`;
   - `data-sketch-create-ticket.md`.
2. Rileggi quei tre file: issue L05, contract sketch L06 e data sketch L06.
3. Chiedi orientamento senza modifiche, se usi un tool AI.
4. Tratta ogni file o area suggerita dall'AI come ipotesi.
5. Verifica nella repo ogni file candidato prima di autorizzarlo.
6. Compila la mappa dei punti di intervento (`entry-point-map.md`).
7. Dichiara file ammessi, file dubbi e file vietati.
8. Scegli un primo slice piccolo per il Lab08.
9. Scrivi il prompt patch limitato che userai nel lab.
10. Scrivi la verifica manuale proposta.
11. Prepara il reviewer leggero.
12. Controlla che il pacchetto sia pronto per L08 senza avviare patch.

## Checkpoint Guidati

| Checkpoint | Output minimo | Domanda di controllo |
| --- | --- | --- |
| Import | 3 artefatti in `lavoro-precedente/` | Hai importato solo i file richiesti? |
| Suggerimento AI | lista file/aree candidate | Sono ancora ipotesi? |
| Verifica file | almeno 2 file/aree con evidenza | Cosa hai letto davvero? |
| File vietati | almeno 2 esclusioni | Cosa impedisce scope creep? |
| Prompt patch | task, file, fuori scope / non-obiettivi (non-goals), verifica, stop | Il builder sa quando fermarsi? |
| Controllo qualita' | reviewer leggero | Il reviewer controlla il diff senza proporre nuove feature? |

## Vincoli

- Non scrivere codice.
- Non aprire PR.
- Non avviare patch in L07.
- Non accettare file suggeriti dall'AI senza verifica.
- Non aggiungere auth, allegati, notifiche, owner avanzato, dashboard o migration.
- Non trasformare il reviewer in un progettista di nuove feature.

## Criteri Di Accettazione (Acceptance Criteria) Del Tuo Output

Il pacchetto L07 e' buono quando:

- ogni file candidato ha evidenza;
- ogni file suggerito ma non verificato resta `dubbio` o fuori scope;
- il prompt patch contiene task, scope, file ammessi, fuori scope / non-obiettivi (non-goals), verifica e stop condition;
- il reviewer cerca solo problemi di scope, contract e verifica;
- L08 puo' partire senza ridiscutere tutto.

## Pronto Quando

Hai finito quando puoi rispondere:

```txt
Quali file ho letto davvero?
Che evidenza ho trovato?
Cosa posso toccare nel primo slice?
Cosa non devo toccare ora?
Quale prompt patch usero' nel lab?
Che cosa controlla il reviewer sul diff?
```

## Cosa Porti Nel Lab08

Nel Lab08 userai questi output prodotti qui:

```txt
output/entry-point-map.md
output/prompt-patch-limitato.md
output/reviewer-leggero.md
```

Prima del lab controlla che il pacchetto dica chiaramente:

- quali file o aree hai letto davvero;
- quali file sono ammessi per il primo slice;
- quali file o comportamenti restano vietati;
- quale prompt patch userai;
- quale verifica manuale proporrai;
- quando il tool deve fermarsi.

Se manca uno di questi punti, completa la traccia. Non avviare ancora la patch.

## Micro-Task Post-Lezione

Non c'e' consegna autonoma separata: questo output entra direttamente nel lab L08.

Se devi rifinire qualcosa, limita il lavoro a:

```txt
mappa dei punti di intervento + prompt patch + reviewer leggero
```

Stop:

```txt
non avviare patch prima del lab.
```

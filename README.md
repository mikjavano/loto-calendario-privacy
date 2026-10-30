# Loto Calendario - Release 3 (Aptoide Edition)

## 📌 Descrizione Generale
**Loto Calendario** è un'applicazione avanzata personalizzabile, progettata per gestire appuntamenti,impegni, 
  attività lavorative, scolastiche ecc... . L'applicazione e' progettata per garantire efficienza e rapidità
  nell'uso pratico dell'utente e offre un'interfaccia utente nativa, ottimizzata per schermi di varie dimensioni 
  (smartphone e tablet).

---

## 🔒 Informativa sulla Privacy e Gestione dei Dati (loto-calendario-privacy)

**Ultimo aggiornamento: 28 Ottobre 2026**

La presente informativa descrive le modalità di gestione dell'applicazione **LotoCalendario** in merito alla privacy e al trattamento dei dati degli utenti:

1. **Raccolta dei Dati Personali:**
   L'applicazione **NON** raccoglie, **NON** memorizza, **NON** registra e **NON** trasmette alcun dato personale dell'utente verso server esterni,
   cloud di terze parti o soggetti terzi.

3. **Gestione dei Dati Locali (Memoria Interna ed Esterna):**
   L'applicazione memorizza le informazioni riguardanti gli incarichi, gli appuntamenti o altre note inserite dall'utente **esclusivamente in locale**. 
   Tali dati risiedono nella directory interna di installazione o, per espresso e volontario volere dell'utente, su unità di memoria esterne 
   (come Flash Drive USB o schede SD) gestite tramite il File Manager integrato per operazioni di backup, esportazione o importazione.

4. **Sicurezza:**
   Poiché gli incarichi creati dall'utente sono salvati internamente nella directory di installazione della applicazione stessa in una directory di default,
   in locale, il livello di sicurezza dei dati inseriti è elevato ed è protetto direttamente dalle politiche di isolamento del sistema operativo Android.

---

## 🛡️ Dettaglio Permessi e Autorizzazioni (`AndroidManifest.xml`)

Per soddisfare i requisiti dei comitati di revisione e garantire la massima trasparenza, si specificano di seguito i motivi per cui l'applicazione richiede 
le seguenti autorizzazioni di sistema:

### 1. Gestione della Memoria e Storage (`MANAGE_EXTERNAL_STORAGE`, `READ_EXTERNAL_STORAGE`, `WRITE_EXTERNAL_STORAGE`)
* **Scopo:** L'applicazione include un modulo File Manager proprietario (*Salva con nome* / *Apri file con nome*).
* **Utilizzo: ** 1 Consentire all'utente di salvare in autonomia appuntamenti creati o copie di appuntamenti esistenti all'interno della applicazione,
                   in directory esterne o memorie rimovibili.
			     ** 2 Consentire all'utente di leggere file di testo esterni(contenenti appuntamenti o note) direttamente tramite il File Manager integrato
                   nell'applicazione.

### 2. Dispositivi di Archiviazione Esterni (`USB_PERMISSION`)
* **Scopo:** Interfacciamento con chiavette USB e unità Flash collegate tramite supporto USB TYPE-C.
* **Utilizzo:** Permettere il salvataggio diretto o la lettura di file di testo da dispositivi USB fisici esterni.

### 3. Connettività e Browser (`INTERNET`, Queries `ACTION_VIEW` / `BROWSABLE`)
* **Scopo:** Fruizione della documentazione e supporto utente online (Guida Online).
* **Utilizzo:** L'autorizzazione `INTERNET` e la dichiarazione delle `<queries>` consentono di lanciare in modo sicuro il browser predefinito
    di sistema via `Intent` quando l'utente seleziona l'opzione "Guida via Internet" all'interno del dialog delle guide. L'app **non** usa la 
    rete per inviare dati o telemetria.

---

## ⌛ Changelog e storico Aggiornamenti

1. **Miglioramento della comunicazione con l'utente con l'inserimento
	  di un nuovo Dialog** interattivo per facilitare l'accesso alla guida 
	  online sul sito internet e alla guida ristretta e veloce interna a 
	  Loto calendario.
2. **Rimozione Librerie Orfane:**
      Eseguita una bonifica approfondita del codice sorgente con 
      l'eliminazione delle chiamate a librerie orfane e la rimozione di 
      riferimenti obsoleti all'interno delle classi, alleggerendo l'
      architettura complessiva.
3. **Pulizia dei Log:**
      Rimozione dei Log di debug superflui per garantire 
      performance piu veloci durante l'uso dell'applicazione.
5. **Ottimizzazione visiva del File Manager Integrato:**
      Sistemata l'interfaccia e la disposizione dei comandi 
      ( come i pulsanti copia/incolla che di fatto non sono funzionanti ) 
      evitando la visualizzazione di pulsanti in fase di sviluppo e 
      risolvendo un problema di allineamento per cui alcuni comandi 
      venivano tagliati fuori dallo schermo sui dispositivi con 
      risoluzioni particolari.
    
---
Documentazione e specifiche tecniche aggiornate in conformità con il
rilascio della versione 3.0  del pacchetto software Loto Calendario.

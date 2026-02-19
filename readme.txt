# Sito Web DEKO Srl - Documentazione Tecnica

## Panoramica Generale
Sito web aziendale per DEKO Srl, specializzata in rivestimenti antiaderenti per cookware e industria. Il sito presenta una palette cromatica basata sui colori della bandiera brasiliana (Verde #009C3B, Giallo #FFDF00, Blu #002776) e include pagine Home, Contatti, Privacy Policy e Cookie Policy.

---

## 📁 Struttura dei File CSS

### `tema.css`
**File principale delle variabili e stili di base**
- Definisce il font personalizzato 'din-2014'
- Imposta le variabili CSS root con la palette colori brasiliana
- Configura lo sfondo nero e i colori del testo
- Definisce classi utility (.text-verde, .bg-giallo, .btn, ecc.)
- Imposta i bottoni principali (primary, ghost) con effetti hover
- Gestisce il layout base e i reset CSS

### `header.css`
**Stili per l'header fisso del sito**
- Header posizionato fixed in alto (100px di altezza)
- Sfondo semitrasparente con effetto blur
- Bordo e ombra verde costante
- Logo con effetto glow e bordo giallo
- Navigazione principale con effetti hover
- Responsive per mobile (altezza ridotta a 80px)

### `footer.css`
**Stili per il footer del sito**
- Sfondo scuro (#0a0a0a) con bordo superiore giallo tenue
- Layout flex per organizzare le informazioni legali
- Testo del copyright e dati aziendali
- Link a Privacy Policy e Cookie Policy con separatori
- Design responsive per mobile

### `home.css`
**Stili specifici per la homepage**
- Hero section con titolo animato e sfumature verdi
- Pulsante CTA con effetti hover
- Griglia a 3 colonne per mostrare catalogo, news ed eventi
- Card interattive con effetti hover e animazioni
- Badge colorati per categorizzare i contenuti
- Animazioni fade-in per gli elementi della griglia

### `contatti.css`
**Stili esclusivi per la pagina Contatti**
- Hero section con titolo grande e accenti verdi
- Griglia di card di contatto (3 colonne)
- Card con effetti hover e gradienti
- Stili specifici per:
  - Indirizzo aziendale
  - Orari di apertura
  - Link email e telefono
- Design completamente responsive

### `policy.css`
**Stili per le pagine Privacy Policy e Cookie Policy**
- Layout pulito e leggibile
- Hero section con gradienti verdi
- Card di contenuto su sfondo scuro
- Tipografia ottimizzata per testi lunghi
- Liste stilizzate e note evidenziate
- Responsive per dispositivi mobili

### `silktide-consent-manager.css`
**Stili per il banner dei cookie (Silktide)**
- Gestione completa del banner cookie
- Variabili CSS per personalizzazione colori
- Stili per il modal delle preferenze
- Switch toggle per accettare/rifiutare cookie
- Animazioni di apertura/chiusura
- Design responsive e accessibile

---

## 📁 Struttura dei File JavaScript

### `main.js`
**File principale JavaScript - Caricamento parziali e interazioni**
- Carica dinamicamente header e footer in base alla lingua
- Gestisce il cambio lingua (IT/EN)
- Imposta la classe active nei link di navigazione
- Gestisce menu off-canvas e submenu
- Controlla header hide/show allo scroll
- Gestisce video hero con autoplay
- Slider infinito per le news
- Lightbox per le immagini
- Ottimizzazioni per Safari mobile

### `index.js`
**Versione semplificata per il caricamento base**
- Carica header e footer tramite fetch
- Gestisce errori di caricamento
- Imposta link attivi nella navigazione
- Versione più leggera per pagine semplici

### `consent-config.js`
**Configurazione del consenso cookie (GDPR)**
- Configura Plausible Analytics (GDPR-compliant)
- Prepara Google Analytics 4 (inattivo di default)
- Imposta Google Consent Mode con default 'denied'
- Configura il banner Silktide con:
  - Cookie necessari (sempre attivi)
  - Cookie analytics (opzionali)
  - Callback onAccept/onReject
  - Testi personalizzati in italiano
- Posiziona il banner in basso a destra

### `silktide-consent-manager.js`
**Libreria completa per la gestione dei cookie**
- Classe principale SilktideCookieBanner
- Gestisce:
  - Creazione banner/modal/icona
  - Salvataggio preferenze in localStorage
  - Focus trap per accessibilità
  - Callback per accettazione/rifiuto
  - Animazioni di transizione
- API pubblica per configurazione dinamica

---

## 📄 File HTML

### `index.html` (Homepage)
**Pagina principale del sito**
- Hero section con titolo e CTA
- Griglia 3 colonne con:
  - Link al catalogo PDF 2026
  - Link a Deko Kustom
  - Link alla sezione azienda
- Header e footer inclusi staticamente
- Meta tag e favicon

### `contatti.html`
**Pagina contatti aziendali**
- Hero section con titolo
- Card informazioni:
  - Indirizzo completo
  - Orari di apertura dettagliati
  - Email e telefono con link diretti
- Design responsive con animazioni

### `privacy-policy.html` (contenuto nel file index.html con titolo Privacy Policy)
**Informativa privacy completa (GDPR)**
- 8 sezioni informative:
  1. Premessa e introduzione
  2. Titolare del trattamento
  3. Categorie di dati trattati
  4. Cookie (rimando a policy specifica)
  5. Finalità del trattamento
  6. Destinatari dei dati
  7. Periodo di conservazione
  8. Diritti dell'interessato
  9. Conferimento dei dati
- Data ultimo aggiornamento: 26/02/2021

### `cookie-policy.html` (contenuto nel file index.html con titolo Cookie Policy)
**Informativa dettagliata sui cookie**
- Gestione dei cookie dal browser
- Cosa sono i cookie
- Tipologie di cookie:
  - Di sessione
  - Persistenti
  - Tecnici
  - Di profilazione
  - Prima/terza parte
- Cookie utilizzati nel sito:
  - Navigazione (indispensabili)
  - Funzionali
  - Analitici
- Istruzioni per disabilitare i cookie

---

## 🎨 Caratteristiche Tecniche

### Design System
- **Colori primari**: Verde (#009C3B), Giallo (#FFDF00), Blu (#002776)
- **Sfondo**: Nero (#000000) per tutto il sito
- **Tipografia**: Font personalizzato 'din-2014'
- **Effetti**: Glow, ombre, gradienti, transizioni fluide

### Funzionalità Interattive
- Header dinamico che si nasconde allo scroll
- Card con effetti hover e animazioni
- Lightbox per immagini
- Gestione consenso cookie GDPR-compliant
- Design completamente responsive
- Accessibilità (attributi ARIA, focus visibile)

### Performance e SEO
- Caricamento differito degli script (defer)
- Ottimizzazione per mobile
- Meta tag e favicon
- Struttura semantica HTML5

---

## 🔧 Manutenzione e Aggiornamenti

### Per aggiornare i contenuti:
1. **Testo**: Modificare direttamente nei file HTML
2. **Cookie/Privacy**: Aggiornare le date e i testi nei file policy
3. **Colori**: Modificare le variabili CSS in `tema.css`
4. **Analytics**: Aggiornare GA4_ID in `consent-config.js`

### Per aggiungere pagine:
1. Creare nuovo file HTML
2. Includere header/footer (statici o tramite JS)
3. Collegare CSS specifici se necessario
4. Aggiornare la navigazione in header

---

## 📱 Compatibilità Browser
- Chrome/Firefox/Safari/Edge (ultime versioni)
- Safari iOS (ottimizzato per autoplay video)
- Dispositivi mobile (responsive breakpoints a 900px e 600px)

---

## 🔒 Conformità GDPR
- Banner cookie con consenso esplicito
- Google Consent Mode integrato
- Possibilità di revocare il consenso
- Informativa privacy completa
- Cookie policy dettagliata
- Solo analytics GDPR-compliant (Plausible)
- GA4 opzionale e configurabile
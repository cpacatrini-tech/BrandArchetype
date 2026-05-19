Chestionar Profil Arhetipal de Brand

Acest proiect este o aplicație web interactivă de tip diagnostic (Lead Generation), dezvoltată în React. Ajută companiile și antreprenorii să își descopere energia de bază (Ethos) și arhetipul dominant al brandului lor, comparând rezultatele cu o bază de date (benchmark) globală.

🎯 Funcționalități Principale

Structură în 2 Valuri: - Valul 1 (Q1-Q3): Determină Ethos-ul (energia nativă a brandului).

Valul 2 (Q4-Q6): Filtrează și expune doar variantele de răspuns specifice Ethos-ului câștigător, determinând Arhetipul final.

Sistem Inteligent de Fallback: Dacă Valul 1 nu generează un Ethos clar (egalitate), Valul 2 va afișa toate cele 12 arhetipuri pentru o calibrare completă.

Diagnostic Cultural: Întrebarea 6 verifică gradul de aliniere dintre cultura internă a echipei și proiecția externă a brandului.

Vizualizare Datelor (Radar Chart): Generează automat un grafic de tip pânză de păianjen care suprapune scorul curent peste o medie globală (benchmark).

Insights Strategice: Oferă interpretări textuale bazate pe scorul obținut (ex: Brand slab conturat vs. Brand puternic).

🛠️ Tehnologii Folosite

React.js (Interfață și logică de stare)

Tailwind CSS (Design și responsivitate)

Recharts (Graficul Radar interactiv)

Lucide-React (Iconițe vectoriale)

Firebase Firestore (Bază de date anonimă pentru salvarea scorurilor și generarea benchmark-ului)

🚀 Cum se utilizează / integrează

Varianta 1: Integrare directă pe site via Iframe (Recomandat)

Dacă aplicația a fost deja publicată pe o platformă de hosting (ex: Vercel, Netlify), ea poate fi integrată pe orice website (WordPress, Webflow, custom) folosind următorul cod:

<iframe 
  src="[https://LINKUL-APLICATIEI-TALE.vercel.app](https://LINKUL-APLICATIEI-TALE.vercel.app)" 
  width="100%" 
  height="850px" 
  style="border:none; border-radius: 12px; box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1);"
  title="Chestionar Arhetip Brand"
></iframe>


Varianta 2: Rulare și dezvoltare locală (Pentru Developeri)

Dacă doriți să modificați codul sau să rulați proiectul local:

Clonați proiectul și instalați dependințele:

npx create-vite chestionar-brand --template react
cd chestionar-brand
npm install recharts lucide-react firebase tailwindcss


Adăugați logica aplicației:
Înlocuiți conținutul din src/App.jsx cu codul din acest proiect.

Porniți serverul de dezvoltare:

npm run dev


Compilare pentru producție:

npm run build


Fișierele finale gata de încărcat pe server vor fi generate în folderul dist.

🎨 Arhitectura Arhetipurilor

Sistemul se bazează pe cele 12 arhetipuri Jungiene, împărțite în 4 axe de Ethos:

Leaving a Thumbprint (Amprentă): Erou, Rebel, Magician

Yearning for Paradise (Paradis): Inocent, Explorator, Înțelept

No man is an island (Conexiune): Om obișnuit, Iubitor, Bufon

Providing structure (Structură): Creator, Ocrotitor, Lider

🔒 Confidențialitate

Datele sunt colectate strict sub formă de scoruri cantitative complet anonime, folosite exclusiv pentru generarea mediei (benchmark-ului) vizibile în graficul final. Nu se colectează date cu caracter personal (PII).

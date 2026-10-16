# Task_apsw_Vlad.F-Alex.B-Ilie.G

Test practic la disciplina **Asistență pentru programarea site-urilor web (APSW)**, realizat pe baza aplicației TaskFlow.

## Echipa

| Nr. | Nume   | Prenume | În numele repo-ului | Cont GitHub                                     | Rol în repository |
|-----|--------|---------|---------------------|-------------------------------------------------|-------------------|
| 1   | Fulga  | Vlad    | `Vlad.F`            | [Vuvucito06](https://github.com/Vuvucito06)     | Proprietar        |
| 2   | Batlan | Alex    | `Alex.B`            | [5SSHift](https://github.com/5SSHift)           | Colaborator       |
| 3   | Ghetan | Ilie    | `Ilie.G`            | [Ghetan-Ilie](https://github.com/Ghetan-Ilie)   | Colaborator       |

Numele repository-ului (`task_apsw_Vlad.F-Alex.B-Ilie.G`) este format din prenumele și inițiala numelui de familie ale fiecărui membru al echipei.

> **Starea proiectului:** toate cele 10 bug-uri sunt reparate (#1–#3 Vlad, #4–#7 Alex, #8–#10 Ilie), iar funcționalitatea nouă (filtrul după prioritate) este implementată. Rămâne verificarea finală pe `main` (#12, Vlad). Progresul se vede în tabelul de mai jos și în [milestone-ul „Evaluare TaskFlow”](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/milestone/1).

## Cum lucrăm în echipă

1. **Acceptați invitația** de colaborator primită pe GitHub (pe email sau la [pagina de invitații](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/invitations)).
2. **Clonați repository-ul echipei.** Fiind colaboratori, nu aveți nevoie de fork:

   ```bash
   git clone https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G.git
   cd task_apsw_Vlad.F-Alex.B-Ilie.G
   npm install
   ```

3. **Lucrați doar pe issue-urile voastre.** Fiecare bug are un issue pe GitHub atribuit unui membru al echipei (vezi tabelul de mai jos), ca doi colegi să nu repare aceeași problemă.
4. **Lucrați pe un branch propriu**, niciodată direct pe `main`:

   ```bash
   git checkout main
   git pull
   git checkout -b fix/<prenume>-<descriere-scurta>   # exemplu: fix/ilie-status-filter
   ```

5. **Faceți commit și push**, apoi deschideți un Pull Request către `main`. Un coleg verifică PR-ul înainte de merge.

## Bug-uri identificate

Fiecare bug are un issue pe GitHub cu pașii de reproducere, comportamentul așteptat și fișierul în care se află problema. Detaliile de testare se trec în PR, folosind [docs/TESTING_TEMPLATE.md](docs/TESTING_TEMPLATE.md).

| Issue | Descriere scurtă | Fișier | Responsabil | Status | PR |
|-------|------------------|--------|-------------|--------|----|
| [#1](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/1) | Filtrul de status „In progress” nu afișează nicio sarcină | `src/pages/Tasks.jsx` | Fulga Vlad | ✅ Rezolvat | [#13](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pull/13) |
| [#2](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/2) | Căutarea după persoană ține cont de majuscule | `src/pages/Tasks.jsx` | Fulga Vlad | ✅ Rezolvat | [#13](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pull/13) |
| [#3](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/3) | Contorul de sarcini din meniul lateral este mereu „7” | `src/App.jsx` | Fulga Vlad | ✅ Rezolvat | [#13](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pull/13) |
| [#4](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/4) | Cardul „In progress” din Dashboard arată mereu 0 | `src/pages/Dashboard.jsx` | Batlan Alex | ✅ Rezolvat | [`fix/alex-dashboard-projects`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Falex-dashboard-projects) |
| [#5](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/5) | Linkul „View all” din Dashboard duce înapoi la Overview | `src/pages/Dashboard.jsx` | Batlan Alex | ✅ Rezolvat | [`fix/alex-dashboard-projects`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Falex-dashboard-projects) |
| [#6](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/6) | Butonul „View project” duce înapoi la Overview | `src/pages/Projects.jsx` | Batlan Alex | ✅ Rezolvat | [`fix/alex-dashboard-projects`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Falex-dashboard-projects) |
| [#7](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/7) | Dashboard și Projects nu afișează eroare când API-ul nu răspunde | `src/pages/Dashboard.jsx`, `src/pages/Projects.jsx` | Batlan Alex | ✅ Rezolvat | [`fix/alex-dashboard-projects`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Falex-dashboard-projects) |
| [#8](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/8) | După ștergerea unei sarcini se ajunge pe Overview, nu în lista de sarcini | `src/pages/TaskDetails.jsx` | Ghetan Ilie | ✅ Rezolvat | [`fix/ilie-task-details`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Filie-task-details) |
| [#9](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/9) | După editare, sarcina își pierde proiectul | `src/pages/TaskDetails.jsx` | Ghetan Ilie | ✅ Rezolvat | [`fix/ilie-task-details`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Filie-task-details) |
| [#10](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/10) | Formularul acceptă un titlu format doar din spații | `src/components/TaskForm.jsx` | Ghetan Ilie | ✅ Rezolvat | [`fix/ilie-task-details`](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pulls?q=is%3Apr+head%3Afix%2Filie-task-details) |

### Alte sarcini

| Issue | Descriere | Responsabil | Status | PR |
|-------|-----------|-------------|--------|----|
| [#11](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/11) | Funcționalitatea nouă: filtru după prioritate pe pagina Tasks | Fulga Vlad | ✅ Implementat | [#13](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/pull/13) |
| [#12](https://github.com/Vuvucito06/task_apsw_Vlad.F-Alex.B-Ilie.G/issues/12) | Testare finală și jurnalul de testare pentru PR | Fulga Vlad | ⏳ Deschis (după #1–#11) | — |

## Ce am rezolvat

### Fulga Vlad (Vuvucito06): pagina Tasks

| Issue | Ce s-a schimbat | Cum s-a verificat |
|-------|-----------------|-------------------|
| #1 | Filtrul compară direct statusul ales cu cel din date. Înainte transforma „In progress” în „In Progress”, valoare care nu există în `db.json`. | „In progress” afișează 2 sarcini; To do 3, Review 1, Done 1, All status 7. |
| #2 | Căutarea compară și numele persoanei cu litere mici și ignoră spațiile de la capete. O sarcină fără persoană nu mai poate produce erori. | `ana`, `Ana`, `ANA` și `  ana  ` găsesc aceleași 2 sarcini; căutarea după titlu funcționează în continuare. |
| #3 | Contorul vine din API și se reîncarcă la fiecare schimbare de pagină. Dacă API-ul nu răspunde, contorul este ascuns. | 7 la pornire, 8 după crearea unei sarcini, 7 după ștergere; ascuns cu API-ul oprit. |
| #11 | Filtru nou „Filter by priority” (All priorities / Low / Medium / High) lângă filtrul de status și un buton „Clear filters” în bara de filtre, vizibil când un filtru este activ. | Combinat cu căutarea și statusul (High + To do + „irina” → 1 sarcină), „Showing X of Y” corect, stare goală pentru Low + Review, resetare din ambele butoane, afișare corectă pe mobil. |

Verificările au fost făcute în browser (Chromium), pe o copie a `db.json`. `npm run build` rulează fără erori.

### Ghetan Ilie (Ghetan-Ilie): detaliile sarcinii și formularul

| Issue | Ce s-a schimbat | Cum s-a verificat |
|-------|-----------------|-------------------|
| #8 | După ștergere, aplicația navighează la `/tasks`. Înainte naviga la `/task`, rută care nu există, așa că ajungeai pe Overview. | Ștergere confirmată → lista de sarcini, fără sarcina ștearsă; „Cancel” la confirmare → sarcina rămâne. |
| #9 | La salvarea editării, `projectId` este convertit în număr cu `Number(...)`, la fel ca la creare. Înainte se salva ca text („2”), iar sarcina nu mai era găsită la niciun proiect. | După mutarea unei sarcini în alt proiect, detaliile, lista Tasks și pagina proiectului arată proiectul nou; în `db.json`, `projectId` rămâne număr. |
| #10 | Titlul este verificat după eliminarea spațiilor de la capete (`trim()`) și se salvează fără ele. | Titlu gol sau doar spații → „A task title is required.”, fără nicio cerere către API, atât la creare, cât și la editare; „   Titlu valid   ” se salvează ca „Titlu valid”. |

Verificările au fost făcute în browser (Chromium), pe o copie a `db.json`, împreună cu verificările lui Vlad, care trec în continuare. `npm run build` rulează fără erori.

### Batlan Alex (5SSHift): Dashboard și Projects

| Issue | Ce s-a schimbat | Cum s-a verificat |
|-------|-----------------|-------------------|
| #4 | Cardul „In progress” numără sarcinile cu statusul `In progress`. Înainte căuta `In Progress` (cu P mare), valoare care nu există în `db.json`. | Cardul arată 2; devine 3 când o sarcină trece în „In progress” și revine la 2 când iese. |
| #5 | Linkul „View all” din „Recent tasks” duce la `/tasks`. Înainte ducea la `/task`, rută care nu există, așa că rămâneai pe Overview. | „View all” deschide lista de sarcini, iar în meniul lateral este evidențiat Tasks. |
| #6 | Butonul „View project” duce la `/projects/:id`. Înainte ducea la `/project/:id`, rută care nu există. | Fiecare dintre cele 3 proiecte deschide pagina lui, cu titlul și sarcinile corecte. |
| #7 | Dashboard și Projects tratează eroarea la încărcare (`.catch()`) și afișează un mesaj clar, ca pagina Tasks. Pe Dashboard statisticile arată „—” în loc de 0, iar textul „No tasks yet” nu mai apare; pe Projects nu mai apare „0 active projects”. | Cu API-ul oprit, ambele pagini afișează mesajul de eroare și nu mai apare `Uncaught (in promise)` în consolă. Cu API-ul pornit, paginile funcționează ca înainte. |

Verificările au fost făcute în browser (Chromium), pe o copie a `db.json`, împreună cu verificările lui Vlad și Ilie, care trec în continuare. `npm run build` rulează fără erori.

## Pornire rapidă

```bash
npm install     # instalează dependențele
npm run api     # terminal 1: API-ul JSON Server pe http://localhost:3001
npm run dev     # terminal 2: aplicația React pe http://localhost:5173
```

Proiectul a fost verificat cu Node.js 22 și npm 11. `npm run build` rulează fără erori.

## Structura proiectului

```text
├── db.json                 # datele de test (proiecte și sarcini) servite de JSON Server
├── docs/
│   └── TESTING_TEMPLATE.md # șablonul jurnalului de testare pentru Pull Request
├── index.html              # pagina HTML în care se montează aplicația
├── package.json            # scripturi npm și dependențe
├── vite.config.js          # configurația Vite
└── src/
    ├── main.jsx            # punctul de intrare React + BrowserRouter
    ├── App.jsx             # layout-ul (sidebar, topbar) și rutele aplicației
    ├── api.js              # funcțiile de comunicare cu API-ul REST
    ├── styles.css          # stilurile aplicației
    ├── components/         # componente reutilizabile (formular, badge-uri, titluri)
    └── pages/              # paginile: Dashboard, Tasks, TaskDetails, NewTask, Projects, ProjectDetails
```

---

_Mai jos este enunțul original al evaluării, primit de la cadrul didactic. Pentru lucrul în echipă, pașii din „Cum lucrăm în echipă” înlocuiesc partea de fork._

# TaskFlow — proiect de evaluare

TaskFlow este o aplicație React pentru gestionarea proiectelor și sarcinilor unei echipe. Repository-ul este folosit pentru o evaluare practică la disciplina **Asistență pentru programarea site-urilor web**.

## Scopul evaluării

Pornind de la aplicația existentă, fiecare student trebuie să:

1. investigheze aplicația și să identifice **10 bug-uri/erori**;
2. reproducă și să corecteze fiecare problemă;
3. implementeze funcționalitatea suplimentară descrisă mai jos;
4. verifice aplicația și să documenteze modificările;
5. trimită soluția printr-un Pull Request către repository-ul personal derivat din proiectul inițial.

Nu modificați direct repository-ul cadrului didactic. Lucrați în propriul fork.

## Tehnologii

- React + Vite
- React Router
- JSON Server ca API REST local
- Lucide React pentru pictograme
- CSS responsive, fără framework CSS suplimentar

## Cerințe tehnice

- Node.js 18+ și npm instalate.
- Git instalat.
- Un cont GitHub.

## Instalare și pornire

Clonați propriul fork, apoi instalați dependențele:

```bash
npm install
```

Porniți API-ul într-un terminal:

```bash
npm run api
```

API-ul va fi disponibil la `http://localhost:3001`.

Porniți aplicația într-un al doilea terminal:

```bash
npm run dev
```

Deschideți URL-ul local afișat de Vite, de regulă `http://localhost:5173`.

Pentru verificarea build-ului:

```bash
npm run build
```

> API-ul trebuie să ruleze separat de serverul Vite. Datele de test se află în `db.json`; operațiile de creare, editare și ștergere modifică acest fișier prin JSON Server.

## Funcționalități existente

- Dashboard cu statistici și sarcini recente.
- Listă de sarcini cu căutare și filtre.
- Vizualizarea detaliilor unei sarcini.
- Crearea, editarea și ștergerea sarcinilor prin API.
- Listă de proiecte și pagină de detalii a proiectului.
- Navigare între pagini prin React Router.
- Date inițiale pentru testare în `db.json`.

Unele comportamente ale aplicației nu funcționează corect intenționat. Investigați aplicația prin utilizare, inspectarea codului și verificarea cererilor API.

## Funcționalitatea suplimentară de implementat

### Filtrare și organizare după prioritate

Implementați o opțiune completă de filtrare a sarcinilor după prioritate: **Low, Medium, High**.

Criterii de acceptare:

- utilizatorul poate selecta o prioritate sau „Toate prioritățile”;
- filtrul funcționează împreună cu căutarea și filtrul după status, fără ca un criteriu să îl anuleze pe celălalt;
- numărul sarcinilor afișate corespunde rezultatului filtrat;
- starea goală este afișată când nu există rezultate;
- controlul are etichetă accesibilă și stil vizual coerent cu aplicația;
- filtrele pot fi resetate ușor.

Nu este suficient să adăugați doar un element vizual: filtrarea trebuie să funcționeze efectiv.

## Flux GitHub obligatoriu

### 1. Fork și clonare

1. Deschideți repository-ul inițial furnizat de cadrul didactic.
2. Apăsați **Fork** pentru a crea o copie în contul propriu.
3. Clonați fork-ul:

```bash
git clone https://github.com/USERNAME/taskflow-evaluare.git
cd taskflow-evaluare
npm install
```

Înlocuiți `USERNAME` cu numele contului vostru GitHub.

### 2. Creați un branch de lucru

```bash
git checkout -b feature/fix-taskflow
```

Lucrați pe acest branch, nu direct pe `main`.

### 3. Salvați modificările prin commit-uri clare

Exemple de mesaje de commit:

```bash
git add .
git commit -m "fix: correct task status filtering"
git commit -m "fix: validate task form"
git commit -m "feat: add priority filter"
```

Fiecare commit trebuie să reprezinte o schimbare logică. Nu este obligatoriu să folosiți exact aceste mesaje, dar mesajele trebuie să fie explicite.

### 4. Publicați branch-ul

```bash
git push -u origin feature/fix-taskflow
```

### 5. Deschideți Pull Request

Din GitHub, creați un Pull Request din branch-ul de lucru către `main` din propriul fork. Dacă cadrul didactic solicită explicit un PR către repository-ul inițial, selectați repository-ul cadrului didactic ca bază.

Titlu recomandat: `Evaluare TaskFlow — Nume Prenume`

În descriere includeți:

- lista celor 10 bug-uri identificate;
- pașii prin care ați reprodus fiecare problemă;
- explicația soluției aplicate;
- descrierea funcționalității noi;
- verificările manuale și comenzile de testare executate;
- eventuale limitări rămase.

## Livrabile

- Fork GitHub cu istoricul commit-urilor.
- Branch de lucru.
- Pull Request completat.
- Cod funcțional și formatat.
- Descrierea celor 10 bug-uri și a soluțiilor.
- Funcționalitatea suplimentară implementată.
- Build fără erori.

## Reguli de lucru

- Nu eliminați funcționalități existente pentru a evita repararea lor.
- Nu înlocuiți API-ul cu date hardcodate în componente.
- Nu includeți fișierele `node_modules` sau `dist` în Git.
- Testați și scenariile cu liste goale, date invalide și răspunsuri API eșuate.
- Codul trebuie să fie lizibil și împărțit logic în componente.
- Fiecare student trebuie să lucreze individual și să poată explica propriile modificări.

## Criterii de evaluare

Baremul detaliat este comunicat de cadrul didactic. Evaluarea ia în considerare corectitudinea remedierilor, calitatea implementării, utilizarea API-ului, navigarea, testarea și calitatea Pull Request-ului.

#  Aplicație Java – Gestionare Produse și Stocuri

##  Introducere
Această aplicație Java oferă o soluție simplă și eficientă pentru gestionarea produselor și a stocurilor, cu autentificare utilizator și conexiune la o bază de date (MySQL sau MongoDB). Scopul principal este identificarea produselor cu stoc redus, folosind o interfață grafică realizată cu Swing.

##  Motivație
Aplicația răspunde nevoii frecvente a magazinelor și depozitelor de a urmări produsele cu stoc scăzut și de a permite utilizatorilor să gestioneze produsele în mod organizat.

---

##  Fundamente teoretice
- **Java OOP**: utilizarea claselor, moștenirii, compunerii și a metodelor suprascrise
- **JDBC / MongoDB**: conectare, interogare și manipulare a bazelor de date
- **Proceduri stocate (MySQL)**: logica business mutată în serverul SQL
- **Swing**: interfață grafică simplă, cu `JFrame`, `JPanel`, `JButton`, `JOptionPane`

---

##  Descrierea problemei
Scopul este de a crea o aplicație care permite:
- Înregistrarea și autentificarea utilizatorilor
- Afișarea produselor din baza de date
- Semnalarea produselor cu stoc redus (sub un prag setat dinamic de utilizator)

---

##  Soluția propusă

###  Tehnologii utilizate
- **Java 17**
- **Swing** pentru interfața grafică
- **MySQL 8.0 / MongoDB** pentru persistarea datelor
- **JDBC** pentru MySQL / **MongoDB Java Driver** pentru MongoDB

###  Structură
- model/ # Clase pentru produse și utilizatori
- dao/ # Acces la bazele de date
- gui/ # Interfața grafică (Swing)
- util/ # Conexiuni DB
- Main.java # Lansare aplicație
  
---

##  Prezentarea aplicației

###  Funcționalități
- Autentificare și înregistrare cu validare
- Căutare produse cu stoc sub prag (input dinamic)
- Interfață intuitivă, rezultatele afișate în popup
- Cod modular, ușor de întreținut

###  Arhitectură
Model de tip **Model-View-Controller (MVC)**:
- Model: clasele `Produs`, `Utilizator`
- View: clase Swing pentru interfață
- Controller: clase care coordonează acțiunile butoanelor și accesul la date

# temadecasa_pa
Autor:Bejoiu Roxana-Georgiana
CR11.A
- 1.Enunțul problemei
Avem sarcina de a dezvolta un algoritm pentru un editor de cod
avansat care să corecteze automat erorile de sintaxă din limbajele de
programare. Se presupune că primim o specificație clară a sintaxei
valide a limbajului de programare sub forma unei ”reguli” și un frag-
ment de cod care conține erori de sintaxă, adică nu se conformează
acelei reguli.
Obiectivul nostru este să construim un algoritm care să determine
numărul minim de operații necesare pentru a transforma fragmentul
de cod într-unul care respectă regula dată. Aceste operații pot include
substituiri de caractere, inserții sau ștergeri.
Să luăm un exemplu concret pentru a ilustra problema: să pre-
supunem că avem următoarea regulă de sintaxă pentru declarațiile
de funcții în limbajul de programare:
”Fiecare funcție trebuie să ˆınceapă cu cuvântul cheie ”func”, ur-
mat de numele funcției închis în paranteze.”
Un exemplu de declarație de funcție validă ar fi ”func(myFunction)”.
Fragmentul de cod dat: ”fnuc(myFuncion”
Obiectivul nostru este să găsim numărul minim de operații nece-
sare pentru a corecta fragmentul de cod astfel încât să se potrivească
cu modelul definit de regulă. Aceste operații pot include, de ex-
emplu, inversarea caracterelor ”n” s, i ”u” pentru a obține ”func”,
apoi insert, ia caracterelor lipsă ”t” s, i ”)”, astfel încât să obținem
”func(myFunction)” conform regulii date.
- 2.Instrucțiuni pentru compilarea codului
- În fișierul main.c se realizează citirea unui fragment de cod si a unei reguli de sintaxă introdusă de către utilizator.Calcularea numărului minim  de operații necesare pentru corecția fragmentului de cod este calculat prin intermediul funcției "calculate_the_minimum_number_of_operations".Funcția "reconstruct_corrected_code" este apelată pentru a furniza fragmentul de codul după ce s-au efectuat operațiile necesare corecției.
- În fișierul code_editor.c sunt scrise funcțiile "minimum", "calculate_the_minimum_number_of_operations" și "reconstruct_corrected_code" care folosesc programarea dinamică în conceperea unui editor de cod. Funcția "minimum" returnează minimul dintre trei numere și este apelată în "calculate_the_minimum_number_of_operations" pentru a calcula minimul dintre trei operații posibileȘinserție, ștergere și substituție.Funcția "calculate_the_minimum_number_of_operations" returnează numărul minim de operații care necesită a fi efectuate pentru corecția unui fragment de cod.Funcția "reconstruct_corrected_code" returnează fragmentul de cod după corecția conform regulii de sintaxă.Aceasta execută mai multe operații pentru a ajunge la rezultatul final.Dacă după verificare se remarcă faptul că un cuvânt este corect, acesta se afișează fără a se mai realiza modificări.Dacă într-un cuvânt caracterele corespund, însă sunt așezate în altă ordine, se realizează substituția.În cazul în care se găsește un caracter care nu face parte din cuvântul dat, acesta va fi șters, iar dacă se observă absența unui caracter, acesta va fi inserat.
- In fișierul code_editor.h se declară cele trei funcții folosite de către editorul de cod.
- După compilare, programul va solicita utilizatorului introducerea fragmentului de cod, cât și a regulii de sintaxă care se dorește a fi respectată și va furniza numărul minim de operații necesare corecției și șirul de caractere după operațiile efectuate. 

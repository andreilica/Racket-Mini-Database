

;============================================================================================
;=                         Tabela Studenți                                                   =
;= +----------------+-----------+---------+-------+-------+                                  =
;= | Număr matricol |   Nume    | Prenume | Grupă | Medie |                                  =
;= +----------------+-----------+---------+-------+-------+                                  =
;= |            123 | Ionescu   | Gigel   | 321CA |  9.82 |                                  =
;= |            124 | Popescu   | Maria   | 321CB |  9.91 |                                  =
;= |            125 | Popa      | Ionel   | 321CC |  9.99 |                                  =
;= |            126 | Georgescu | Ioana   | 321CD |  9.87 |                                  =
;= +----------------+-----------+---------+-------+-------+                                  =
;=                                                                                           =
;=                                         Tabela Cursuri                                    =
;= +------+----------+-----------------------------------+---------------+------------+      =
;= | Anul | Semestru |            Disciplină             | Număr credite | Număr teme |      =
;= +------+----------+-----------------------------------+---------------+------------+      =
;= | I    | I        | Programarea calculatoarelor       |             5 |          2 |      =
;= | II   | II       | Paradigme de programare           |             6 |          3 |      =
;= | III  | I        | Algoritmi paraleli și distribuiți |             5 |          3 |      =
;= | IV   | I        | Inteligență artificială           |             6 |          3 |      =
;= | I    | II       | Structuri de date                 |             5 |          3 |      =
;= | III  | II       | Baze de date                      |             5 |          0 |      =
;= +------+----------+-----------------------------------+---------------+------------+      =
;============================================================================================

Modul meu de implementare al bazei de date este urmatorul:

   Baza de date in sine este o lista care contine mai multe liste. Fiecare dintre aceste liste interne reprezinta o tabela.
   Structura unei tabele:
      Primul element al listei este un string ce reprezinta numele acesteia, iar urmatoarele elemente sunt o serie de liste
      ce reprezinta coloanele din tabela. Fiecare dintre aceste liste are pe prima pozitie un string ce reprezinta numele
      coloanei, iar celelalte elemente sunt valorile introduse in tabela pentru acea coloana. Un exemplu cu modul acesta de
      implementare este prezentat mai jos prin apelul ( db ): 
      
'(("Studenți"
   ("Număr matricol" 123 124 125 126)
   ("Nume" "Ionescu" "Popescu" "Popa" "Georgescu")
   ("Prenume" "Gigel" "Maria" "Ionel" "Ioana")
   ("Grupă" "321CA" "321CB" "321CC" "321CD")
   ("Medie" 9.82 9.91 9.99 9.87))

  ("Cursuri"
   ("Anul" "I" "II" "III" "IV" "I" "III")
   ("Semestru" "I" "II" "I" "I" "II" "II")
   ("Disciplină" "Programarea calculatoarelor" "Paradigme de programare" "Algoritmi paraleli și distribuiți" "Inteligență artificială" "Structuri de date" "Baze de date")
   ("Număr credite" 5 6 5 6 5 5)
   ("Număr teme" 2 3 3 3 3 0)))
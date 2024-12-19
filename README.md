# CONCESSIONARIO AUTO USATE

| Nome                  | Tipo           | Attributi                               | Note                                                                 |
| --------------------- | -------------- | --------------------------------------- | -------------------------------------------------------------------- |
| id                    | BIGINT(20)     | PRIMARY KEY - AUTO_INCREMENT - UNSIGNED | BIGINT(20) per convenzione                                           |
| targa                 | CHAR(9)        | NOT NULL - UNIQUE                       | Numero di targa (le targhe più lunghe al mondo hanno 9 caratteri)    |
| targa                 | CHAR(9)        | NOT NULL - UNIQUE                       |
| numero_telaio         | CHAR(17)       | NOT NULL - UNIQUE                       |
| marca                 | VARCHAR(50)    | NOT NULL                                |
| modello               | VARCHAR(50)    | NOT NULL                                |
| anno_immatricolazione | YEAR           | NOT NULL                                |
| chilometraggio        | INT            | NOT NULL                                |
| colore                | VARCHAR(30)    | NULL                                    |
| alimentazione         | VARCHAR(20)    | NULL                                    | Tipo di carburante (benzina, diesel, elettrica, ibrido, ecc.)        |
| cilindrata            | INT            | NULL                                    |
| potenza_cv            | INT            | NULL                                    |
| num_porte             | INT            | NULL                                    |
| prezzo_vendita        | DECIMAL(10, 2) | NULL                                    |
| data_acquisizione     | DATE           | NULL                                    | Data di acquisto dell'auto da parte del concessionario               |
| condizioni            | VARCHAR(255)   | NULL                                    | Condizioni generali dell'auto (es. "buone", "ottime", "da riparare") |
| immagini              | TEXT           | DEFAULT 'placeholder'                   | URL o percorso delle immagini dell'auto                              |
| stato_disponibilità   | VARCHAR(50)    | DEFAULT 'disponibile'                   | Stato attuale dell'auto nel concessionario (es. "disponibile")       |
| note                  | TEXT           | NULL                                    | Note aggiuntive o dettagli specifici dell'auto                       |

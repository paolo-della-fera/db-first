# db-first

Modellizzare la struttura di una tabella per memorizzare tutti i dati riguardanti delle auto usate messe in vendita da un concessionario

<br>
<br>

# Concessionario DB

## Table name: Cars

## Colums

- id                      -> ( BIGINT | INDEX | NOT NULL | AUTO INCREMENT | PRIMARY KEY )
- VIN                     -> ( CHAR(17) | NOT NULL | UNIQUE )
- Casa Automobilistica    -> ( VARCHAR(100) | INDEX | NULL )
- Modello                 -> ( VARCHAR(100) | INDEX | NOT NULL )
- Auto IMG                -> ( VARCHAR(255) | DEFAULT ( link immagine / percorso ) )
- Anno                    -> ( YEAR | NULL)
- Targa                   -> ( CHAR(7) | NULL | UNIQUE)
- Alimentazione           -> ( VARCHAR(20) | INDEX | NOT NULL )
- Tipo di Motore          -> ( VARCHAR(50) | NULL )
- Cavalli                 -> ( SMALLINT | NULL )
- Trasmissione            -> ( VARCHAR(20) | NOT NULL )
- km ( Usato )            -> ( INT | DEFAULT ( 0 ) )
- Colore                  -> ( VARCHAR(50) | NULL )
- Prezzo                   -> ( DECIMAL(10,2) | NOT NULL )
- Stato                   -> ( VARCHAR(20) | INDEX | NULL )
- Condizioni              -> ( VARCHAR(50) | NULL )
- Descrizione             -> ( TEXT | NULL )

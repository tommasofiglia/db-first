<!-- Tabella contenente le informazioni su un negozio di videogioco -->

# database name: GameTom
# table name: Videogames

- id BIGINT PRIMARYKEY NOTNULL
- title string VARCHAR(50) NOTNULL
- descrition string TEXT NULL
- genre string VARCHAR(15) NOTNULL
- front_img VARCHAR() NOTNULL
- retro_img VARCHAR() NOTNULL
- publisher VARCHAR(30) NOTNULL
- developer VARCHAR(30) NOTNULL
- format VARCHAR(10) NOTNULL
- platform VARCHAR(10) NOTNULL
- languages VARCHAR(100) NOTNULL
- edition VARCHAR(10) NULL
- release_year date YEAR
- release_date date DATE NULL
- price FLOAT(6,2) NOTNULL
- availability number TINYINT NULL DEFAULT(1)
- quantity SMALLINT NULL DEFAULT(0)
- pegi SMALLINT NOTNULL
- barcode SMALLINT NOTNULL UNIQUE

<!-- Tabella contenente le informazioni su un negozio di videogioco -->

# database name: GameTom
# table name: Videogames

- id BIGINT PRIMARYKEY NOTNULL
- title               string        VARCHAR(50)     NOTNULL
- descrition          string        TEXT            NULL
- genre               string        VARCHAR(15)     NOTNULL
- front_img           string        VARCHAR()       NOTNULL
- retro_img           string        VARCHAR()       NOTNULL
- publisher           string        VARCHAR(30)     NOTNULL
- developer           string        VARCHAR(30)     NOTNULL
- format              string        VARCHAR(10)     NOTNULL
- platform            string        VARCHAR(10)     NOTNULL
- languages           string        VARCHAR(100)    NOTNULL
- edition             string        VARCHAR(10)     NULL
- release_year        date          YEAR            NOTNULL
- release_date        date          DATE            NULL
- price               number        FLOAT(6,2)      NOTNULL
- availability        number        TINYINT         NULL DEFAULT(1)
- quantity            number        SMALLINT        NULL DEFAULT(0)
- pegi                number        SMALLINT        NOTNULL
- barcode             number        SMALLINT        NOTNULL UNIQUE

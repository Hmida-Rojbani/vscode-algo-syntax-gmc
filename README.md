# algoGMC README

Syntax reader for algorithm language. Code example:
```
FUNCTION Locate_film(name_film : STRING) : INTEGER
    VAR
        i : INTEGER
        not_found : BOOLEAN
    START
        i := 0
        not_found := TRUE
        REPEAT
            IF names[i] = name_film THAN
                not_found := TRUE
            ELSE
                i <- i + 1
            ENDIF
        UNTIL not_found AND i < NB_FILM

        IF not_found THAN
            i := NULL
        ENDIF

        RETRUN i
    END
ENDFUNCTION

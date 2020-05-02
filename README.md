# algoGMC README

Syntax reader for algorithm language. Code example:
```
FUNCTION Locate_film(name_film : INTEGER) : INTEGER 
    VAR
        i : INTEGER;
        not_found : BOOLEAN;
    BEGIN
        i := 0;
        not_found := TRUE;
        REPEAT
            IF names[i] = name_film THAN 
                not_found := TRUE;
            ELSE
                i := i + 1;
            END_IF
        UNTIL not_found AND i < NB_FILM

        IF not_found THAN
            i := NULL;
        END_IF

        RETURN i;
    END
END_FUNCTION



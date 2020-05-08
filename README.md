# algoGMC README

Syntax reader for algorithm language. the extension of the file must be *.algo

Code example 1:
```
ALGORITHM three_nb_sum
VAR
    num1,num2,num3 : INTEGER;
    sum : INTEGER := 0;
BEGIN
    Read(num1);
    Read(num2);
    Read(num3);
    sum := num1 + num2 + num3;
    Write(sum);
END

Code example 2:
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



# Laboratorio 3 - Robótica Industrial 2, Entradas y Salidas
Desarrollado por Daniel Cruz y Cristhian Pulido

## Descripción de la solución planteada
## Explicación del código 

```RAPID
 PROC main()
        Path_inicial;
    	WaitTime 1;
        IF EntDI_1 = 1 THEN
            SetDO SalDO_1,1;
            Path_tdibujo;
            Path_dibujo;
            Path_tdibujo;
            Path_inicial;
        ELSEIF EntDI_2 = 1 THEN
            Path_changeTool;
            SetDO SalDO_1,0;
            WaitDI EntDI_2,1;
            Path_setTool;
        ELSE
            Path_inicial;
        ENDIF
    ENDPROC
```
## Conclusiones

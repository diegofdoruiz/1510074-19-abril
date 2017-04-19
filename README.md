- Solución para mostrar todos los procesos del sistema
- El comando ps -A lista todos los procesos en curso
- El comando ps -A | wc -l muestra el número de procesos en curso

```
ps -A | wc -l
```
- Solución para mostrar 2^4
```
export TOTAL=$((2**4))
echo $TOTAL
```

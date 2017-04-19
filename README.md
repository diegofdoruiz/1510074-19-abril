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
- Solución para condicional
``` 
if [ $VAR2 -eq 3 ]; then
	echo "es igual a 3";
else
	echo "no es igual a 3";
fi
```
- Iterar en un rango de 1 a 10 
```
export RANGO=10
for i in $(seq 1 $RANGO); do echo $i; done
```

- ver el número de procesos sin encabezado
- tail -n +2, muestra a partir de la linea 2
```
ps -A > archivo.txt
cat archivo.txt |  tail -n +2
cat archivo.txt |  tail -n +2 | wc -l
```

- tomar datos de la memoria
```
free | grep Mem |tr -s ' ' | cut -d ' ' -f 2
```

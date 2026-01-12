## Caso Elegido: Notificador del Estado Actual del Tiempo (Buenos Aires, Distrito Federal)

El trigger del workflow es un Schedule Trigger el cual se dispara cada 3 horas.
El primer nodo de accion es el HTTP Responde, el cual conecta con la api de weatherapi y nos devuelve un archivo json 
con las características actuales del tiempo (temperatura, estado, velocidad del viento, humedad, etc).
Luego pasamos al nodo Switch el cual es un condicional que dependiendo del estado del tiempo (lluvioso, nublado, parcialmente nublado o soleado)
redirige el flujo y envia un email personalizado con los datos importantes.

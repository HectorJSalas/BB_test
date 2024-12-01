# BB_test
Data Engineering Test
1. Para los ids nulos ¿Qué sugieres hacer con ellos ?
Generar una segundo datased para validcion de estos ids nulos y verifica si es posible la correcion de estos registros y validar el porque se genero la inconsistencia sobre los regristros
2. Considerando las columnas name y company_id ¿Qué inconsistencias notas
y como las mitigas?
Existen valores nulos para ambos casos , para la columna name existen registros con valores Alpha numericos y en coso de columna id existen valores con caracteres especiales , para mitigar estas inconsistencias,una propuesta seria generar validaciones sobre los campos validar el tipo de registro y aislar los casos particulares de 
3. Para el resto de los campos ¿Encuentras valores atípicos y de ser así cómo
procedes?
Si se encontraron valores atipicos dentro de los siguientes campos:

amount: Valores exesivamente altos, para estos campos , generar un umbral de alertamiento para ideitifar los casos especificaos en los dias que se presenten estos  montos
status:Statu con errores  de sintaxys generar un catlogo de estatus validos para generar una validacion de este campo

created_at: fechas diferentes al formto esperado,generar un proceso que nos permita hacer correciones en caso de tener distintos formatos tratando de unificar los formatos de fecha antes de hacer las conversiones


4. ¿Qué mejoras propondrías a tu proceso ETL para siguientes versiones?
integracions de reglas de negocio , robustecer la validacion de campos
generacion de alarmientos para los distintos casos de validacion , integracion a un sitema de automatizacion , creacion de repositorio para control de versiones por ambiente (dev, qa,prod)
# Hospital_asignacion_box_HGGB
Asignación de boxes ambulatorios: Modelo exacto + GRASP ajustado para asignación de boxes de atención ambulatoria.

---
## Contexto y descripción

En los policlínicos de atención ambulatoria, cada semana los profesionales
de salud tienen una agenda con múltiples actividades distribuidas en bloques
horarios de lunes a viernes, considerando que de lunes a jueves los horarios de atención son desde las 8:00 hasta las 17:00 y los días viernes desde 8:00 hasta 16:00. Cada actividad necesita un box de atención
física para realizarse, y asignarlos manualmente es complejo porque no todos
los boxes son compatibles con todos los tipos de atención, algunos están
reservados para ciertas profesiones, y lo ideal es que cada profesional
permanezca en el mismo box durante el día para no desplazar equipos ni
incomodar al paciente.

Este proyecto aborda ese problema en el policlínico de Cirugía Infantil
del Hospital Guillermo Grant Benavente (Concepción, Chile), implementando
dos enfoques: un modelo de Programación Entera Mixta que encuentra la
solución óptima garantizada, y una metaheurística GRASP que obtiene
soluciones de muy buena calidad sin requerir licencias externas.

---

## Uso académico

Los archivos de este repositorio contienen datos reales anonimizados y
están disponibles para ser utilizados libremente con fines de investigación
y docencia.

**Para reproducir el caso de estudio**, los datos incluidos corresponden
al policlínico real y permiten obtener exactamente los mismos resultados
del estudio original sin necesidad de acceso al hospital.

**Para comparar métodos de solución**, el repositorio ofrece dos
implementaciones sobre la misma instancia: el modelo exacto como
referencia de optimalidad y el GRASP como alternativa práctica,
lo que facilita estudios de comparación de rendimiento.

**Para adaptar el modelo a otro contexto hospitalario**, la configuración
del policlínico está completamente separada del código en los archivos
Excel. Basta con reemplazar esos archivos con los datos de otra
institución para aplicar el mismo método sin tocar el algoritmo.

**Para extender la investigación**, el código es una base sobre la
que se pueden explorar variantes como la incorporación de incertidumbre
en los horarios, la consideración de preferencias de box por profesional,
la comparación con otras metaheurísticas, o la extensión del modelo
a múltiples policlínicos simultáneos.

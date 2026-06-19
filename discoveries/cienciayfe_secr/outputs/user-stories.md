# User stories - cienciayfe_secr

- **[US-01]** Como secretaria academica, quiero cargar la informacion academica en una sola fuente para preparar cuadros finales, promociones y abanderados sin trabajar con archivos dispersos.
  - Criterios de aceptacion:
    - Dado un archivo de datos academicos, cuando lo cargo en el sistema, entonces la informacion queda registrada como fuente central del periodo seleccionado.
    - Dado que existe informacion cargada, cuando consulto el periodo, entonces veo la version vigente disponible para revision.
  - Fuente: secretaria.md

- **[US-02]** Como secretaria academica, quiero detectar inconsistencias en nombres, cursos, promociones y promedios para corregirlas antes de generar documentos oficiales.
  - Criterios de aceptacion:
    - Dado un conjunto de datos cargado, cuando ejecuto la validacion, entonces el sistema lista inconsistencias encontradas en nombres, cursos, promociones y promedios.
    - Dado que existen inconsistencias, cuando reviso el resultado, entonces cada inconsistencia muestra el registro afectado y el tipo de problema.
  - Fuente: secretaria.md

- **[US-03]** Como secretaria academica, quiero validar la informacion necesaria para abanderados para evitar errores en reconocimientos estudiantiles.
  - Criterios de aceptacion:
    - Dado un periodo con datos cargados, cuando ejecuto la validacion de abanderados, entonces el sistema indica si faltan datos o si hay promedios inconsistentes.
    - Dado que la validacion encuentra errores, cuando intento generar el listado final, entonces el sistema advierte que la informacion aun requiere correccion.
  - Fuente: secretaria.md

- **[US-04]** Como rectora, quiero revisar una version validada de cuadros finales, promociones y abanderados para firmar documentos con mayor confianza.
  - Criterios de aceptacion:
    - Dado que secretaria genero documentos desde datos validados, cuando rectoria revisa la version final, entonces puede ver que no existen inconsistencias abiertas.
    - Dado que existen inconsistencias pendientes, cuando se intenta enviar a firma, entonces el sistema muestra que la version no esta lista para firma.
  - Fuente: reectora.md

- **[US-05]** Como secretaria academica, quiero generar cuadros finales y cuadros de promociones desde una version validada para reducir reprocesos y retrasos.
  - Criterios de aceptacion:
    - Dado que la informacion del periodo esta validada, cuando genero los cuadros finales, entonces el sistema produce documentos basados en esa version.
    - Dado que la informacion del periodo no esta validada, cuando intento generar documentos oficiales, entonces el sistema solicita resolver las inconsistencias primero.
  - Fuente: reectora.md

- **[US-06]** Como secretaria academica, quiero identificar cambios o correcciones posteriores a un avance para no seguir trabajando con una version desactualizada.
  - Criterios de aceptacion:
    - Dado que existe un avance generado, cuando se carga una correccion posterior, entonces el sistema marca que el avance debe revisarse nuevamente.
    - Dado que hay cambios posteriores, cuando consulto el estado del documento, entonces veo que la version anterior ya no debe usarse como final.
  - Fuente: secretaria.md

- **[US-07]** Como desarrollador de solucion, quiero que el sistema detecte datos faltantes y estudiantes duplicados para disminuir validaciones manuales.
  - Criterios de aceptacion:
    - Dado un conjunto de datos cargado, cuando ejecuto validaciones tecnicas, entonces el sistema reporta registros incompletos y posibles duplicados.
    - Dado un reporte de validacion, cuando secretaria lo revisa, entonces puede priorizar las correcciones necesarias antes de generar documentos.
  - Fuente: desarrollador.md

- **[US-08]** Como rectora, quiero separar claramente la informacion del periodo 2025-2026 y los avances del periodo 2026-2027 para evitar cruces entre cierres y nuevos procesos.
  - Criterios de aceptacion:
    - Dado que existen datos de mas de un periodo, cuando consulto la informacion, entonces cada registro pertenece a un periodo academico identificable.
    - Dado que se genera un documento, cuando reviso su encabezado o metadatos, entonces el periodo academico aparece claramente asociado al documento.
  - Fuente: reectora.md

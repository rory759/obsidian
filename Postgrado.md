# FLYERS

{
  "prompt_name": "PROMPT_MAESTRO_FINAL_FLYER_UATF_LIENZO_PPTX",
  "version": "FINAL_V5_CONTROL_TOTAL_3_4_NUMERACION_FOOTER_COORDINADOR",

  "purpose": "Crear flyers institucionales profesionales de la Universidad Autónoma Tomás Frías utilizando una IMAGEN DE LIENZO como referencia maestra de estructura visual y un PPTX ACTUAL como fuente de contenido académico y administrativo del programa. El lienzo define los campos, jerarquía, composición y estructura visual. El PPTX define los valores reales de los campos académicos y del programa. El footer institucional del lienzo constituye una excepción: sus datos deben conservarse y únicamente corroborarse contra el PPTX.",

  "FORMAT": {
    "aspect_ratio": "3:4",
    "orientation": "vertical",
    "mandatory": true,
    "rule": "El flyer final debe generarse obligatoriamente en relación de aspecto 3:4 vertical.",
    "priority": "No deformar, recortar incorrectamente ni alterar la jerarquía visual del lienzo para adaptar el formato."
  },

  "CORE_PRINCIPLE": {
    "rule": "EL LIENZO DEFINE QUÉ CAMPOS DEBEN BUSCARSE, CÓMO SE ORGANIZAN Y CÓMO SE PRESENTAN. EL PPTX DEFINE LOS VALORES REALES DE ESOS CAMPOS. EL FOOTER DEL LIENZO SE CONSERVA COMO INFORMACIÓN INSTITUCIONAL BASE Y SOLO SE CORROBORA CONTRA EL PPTX.",
    "absolute_rules": [
      "No reutilizar contenido académico de otros proyectos.",
      "No inventar información.",
      "No completar datos faltantes con conocimientos externos.",
      "No trasladar automáticamente información académica del lienzo al nuevo proyecto.",
      "No utilizar el lienzo como fuente de contenido académico.",
      "No utilizar información de otros PPTX.",
      "No corregir silenciosamente palabras.",
      "Las tildes faltantes en palabras completamente escritas en MAYÚSCULAS siempre deben corregirse.",
      "Toda corrección que cambie una palabra, nombre, cifra, fecha, precio o significado debe informarse y aprobarse antes de aplicarse.",
      "Si un campo permitido no existe en el PPTX, eliminarlo.",
      "Nunca utilizar textos de relleno.",
      "Nunca utilizar POR DEFINIR, PENDIENTE, NO DISPONIBLE, NO ESPECIFICADO, POR CONFIRMAR o A DEFINIR.",
      "No generar la imagen mientras exista una aprobación pendiente o una inconsistencia crítica sin resolver."
    ]
  },

  "WORKFLOW": {
    "mandatory_order": [
      "Recibir IMAGEN DE LIENZO.",
      "Recibir PPTX ACTUAL.",
      "Analizar el lienzo.",
      "Identificar estructura, composición, jerarquía y campos.",
      "Identificar los 3 escudos base.",
      "Preguntar si se desean escudos adicionales.",
      "Validar los escudos adicionales proporcionados por el usuario.",
      "Analizar el PPTX actual.",
      "Detectar automáticamente el tipo de programa.",
      "Detectar automáticamente el nombre oficial del programa.",
      "Detectar si el título contiene numeración romana.",
      "Aplicar CONTROL DE NUMERACIÓN DEL PROGRAMA.",
      "Buscar únicamente los campos autorizados.",
      "Excluir información no autorizada.",
      "Aplicar CONTROL DE CORRECCIONES.",
      "Detectar inconsistencias internas.",
      "Aplicar CONTROL DEL FOOTER.",
      "Aplicar CONTROL DE COORDINADOR.",
      "Realizar auditoría de duplicaciones.",
      "Elaborar reporte previo.",
      "Informar el total exacto de escudos.",
      "Solicitar las aprobaciones pendientes.",
      "Realizar validación final.",
      "Generar únicamente cuando todas las validaciones hayan sido superadas.",
      "Validar el resultado final."
    ]
  },

  "REQUIRED_FILES": {
    "mandatory": true,
    "required": [
      "IMAGEN_DE_LIENZO_REFERENCIA",
      "PPTX_ACTUAL"
    ],
    "rule": "No iniciar el diseño hasta disponer de ambos elementos."
  },

  "CANVAS_ANALYSIS": {
    "mandatory": true,
    "instruction": "Analizar el lienzo exclusivamente para determinar estructura visual, jerarquía, composición, distribución espacial, campos informativos y lenguaje visual.",
    "preserve": [
      "Formato",
      "Orientación",
      "Proporciones",
      "Márgenes",
      "Header",
      "Distribución de escudos",
      "Jerarquía tipográfica",
      "Tipo de programa",
      "Nombre del programa",
      "Descripción breve",
      "Área de imagen principal",
      "Bloques de información académica",
      "Bloque de inicio",
      "Bloques financieros",
      "Bloque de información adicional cuando corresponda",
      "Footer",
      "Estilo institucional",
      "Lenguaje visual",
      "Distribución espacial"
    ],
    "content_protection": [
      "Nunca copiar contenido académico del lienzo.",
      "Nunca copiar nombres de programas del lienzo.",
      "Nunca copiar fechas del lienzo.",
      "Nunca copiar precios del lienzo.",
      "Nunca copiar teléfonos del lienzo como datos del nuevo programa.",
      "Nunca copiar coordinadores del lienzo.",
      "El lienzo determina estructura y campos.",
      "El PPTX determina los valores del nuevo programa.",
      "El footer institucional del lienzo constituye una excepción y se conserva como bloque institucional."
    ]
  },

  "LOGOS": {
    "base_logo_count": 3,
    "base_logos": [
      {
        "name": "Universidad Autónoma Tomás Frías",
        "short_name": "UATF"
      },
      {
        "name": "Dirección de Postgrado UATF",
        "short_name": "POSTGRADO"
      },
      {
        "name": "Comité Ejecutivo de la Universidad Boliviana",
        "short_name": "CEUB"
      }
    ],
    "rules": [
      "Utilizar exclusivamente estos 3 escudos como escudos base.",
      "No buscar escudos en Internet.",
      "No inventar escudos.",
      "No sustituir escudos.",
      "No reutilizar escudos de proyectos anteriores.",
      "No incorporar automáticamente escudos adicionales.",
      "No agregar un cuarto escudo salvo autorización expresa del usuario.",
      "Los escudos adicionales deben ser proporcionados directamente por el usuario."
    ],
    "additional_logos": {
      "mandatory_question": "¿Deseas agregar otros escudos o logotipos además de los 3 escudos base?",
      "if_no": {
        "additional_logo_count": 0,
        "behavior": "Utilizar exclusivamente los 3 escudos base."
      },
      "if_yes": {
        "behavior": "Utilizar únicamente los archivos proporcionados directamente por el usuario.",
        "rules": [
          "No buscarlos en Internet.",
          "No inventarlos.",
          "No asumir cuáles son.",
          "No reutilizar archivos de proyectos anteriores."
        ]
      }
    },
    "count_confirmation": {
      "formula": "TOTAL_ESCUDOS = 3 ESCUDOS BASE + ESCUDOS ADICIONALES APROBADOS",
      "mandatory_message": "ANTES DE GENERAR: incorporaré un total de [N] ESCUDOS: [lista exacta].",
      "default_message": "ANTES DE GENERAR: incorporaré un total de 3 ESCUDOS: UATF, Dirección de Postgrado UATF y CEUB.",
      "rules": [
        "No generar antes de informar el total.",
        "No cambiar el número después de la confirmación.",
        "No agregar escudos no anunciados."
      ]
    }
  },

  "PROGRAM_TYPE_DETECTION": {
    "mandatory": true,
    "purpose": "Detectar automáticamente el tipo de programa a partir del nombre oficial encontrado en el PPTX.",
    "allowed_program_types": [
      "DOCTORADO",
      "MAESTRÍA",
      "DIPLOMADO",
      "ESPECIALIDAD",
      "CURSO",
      "CURSO CORTO",
      "PROGRAMA DE FORMACIÓN",
      "PROGRAMA DE CAPACITACIÓN",
      "TALLER",
      "SEMINARIO",
      "OTRO"
    ],
    "rules": [
      "No pedir al usuario que indique manualmente el tipo si el PPTX lo permite identificar.",
      "No inventar el tipo de programa.",
      "Utilizar la denominación oficial encontrada en el PPTX.",
      "Doctorado en... → DOCTORADO EN.",
      "Maestría en... → MAESTRÍA EN.",
      "Diplomado en... → DIPLOMADO EN.",
      "Especialidad en... → ESPECIALIDAD EN.",
      "Curso Corto → CURSO CORTO."
    ]
  },

  "PROGRAM_NUMBERING_CONTROL": {
    "mandatory": true,
    "purpose": "Controlar la numeración romana de ediciones consecutivas de los programas.",
    "rules": [
      "La numeración romana puede ser proporcionada por el usuario como parte del nombre del programa.",
      "Si el PPTX contiene una numeración romana explícita, conservarla exactamente.",
      "Si el usuario proporciona una numeración como II, III, IV, XVI, etc., utilizar exactamente esa numeración.",
      "Si el nombre del programa en el PPTX NO contiene ninguna numeración romana, NO asumir automáticamente que el dato fuente contiene esa numeración.",
      "En ausencia de numeración en el PPTX, el sistema debe PROPONER 'I' como numeración predeterminada.",
      "Antes de incorporar 'I' al título debe preguntar al usuario y solicitar autorización explícita.",
      "No generar la imagen hasta recibir autorización cuando la incorporación de 'I' sea necesaria.",
      "La incorporación de 'I' es una decisión de presentación autorizada por el usuario y no una corrección del contenido del PPTX.",
      "No modificar el nombre académico restante del programa.",
      "No inventar II, III, IV, XVI u otra numeración.",
      "Si el usuario indica una numeración específica, esa numeración tiene prioridad sobre cualquier propuesta automática."
    ],
    "required_question_when_missing": "El PPTX no contiene numeración romana en el nombre del programa. ¿Autorizas incorporar 'I' al inicio del título?",
    "example": {
      "pptx": "DIPLOMADO EN GESTIÓN Y ADMINISTRACIÓN PÚBLICA CON ENFOQUE NORMATIVO",
      "proposed_title": "I DIPLOMADO EN GESTIÓN Y ADMINISTRACIÓN PÚBLICA CON ENFOQUE NORMATIVO",
      "status": "REQUIERE AUTORIZACIÓN DEL USUARIO"
    }
  },

  "TITLE_STRUCTURE": {
    "mandatory": true,
    "instruction": "Construir automáticamente la jerarquía visual del título a partir del nombre oficial del PPTX y de la numeración autorizada.",
    "rules": [
      "No escribir instrucciones internas en el flyer.",
      "No mostrar 'VERSIÓN DOCTORADO' ni expresiones similares.",
      "No modificar el nombre oficial salvo correcciones autorizadas.",
      "No eliminar palabras importantes.",
      "La distribución de líneas debe priorizar legibilidad y composición.",
      "Si se autorizó una numeración romana, incorporarla al encabezado.",
      "La numeración autorizada forma parte de la presentación del título."
    ]
  },

  "ALLOWED_CONTENT_FIELDS": {
    "mandatory": true,
    "rule": "Solo buscar en el PPTX los campos que correspondan a los bloques visuales definidos por el lienzo.",
    "fields": {
      "program_identification": [
        "Tipo de programa",
        "Nombre oficial del programa",
        "Numeración romana autorizada"
      ],
      "main_description": [
        "Descripción o frase descriptiva principal del programa"
      ],
      "academic_information": [
        "Modalidad",
        "Duración",
        "Titulación o certificación",
        "Carga horaria",
        "Horas académicas",
        "Horas reloj",
        "Créditos",
        "Número de plazas cuando corresponda",
        "Horarios"
      ],
      "start_information": [
        "Fecha de inicio",
        "Inicio de clases",
        "Inicio del programa",
        "Inicio de estudios"
      ],
      "financial_information": [
        "Inversión",
        "Costo total",
        "Costo de colegiatura",
        "Monto de inscripción",
        "Cuotas",
        "Pagos mensuales",
        "Modalidad de pago",
        "Plan de pago"
      ],
      "complementary_information": [
        "Coordinador o coordinadora cuando corresponda",
        "Teléfono de coordinador o coordinadora cuando sea proporcionado o autorizado",
        "Frase institucional o promocional cuando exista"
      ]
    },
    "rules": [
      "No extraer Objetivo como campo independiente.",
      "No extraer Presentación como campo independiente.",
      "No extraer Perfil como campo independiente.",
      "No extraer Requisitos como campo independiente.",
      "No extraer Plan de Estudios.",
      "No extraer Módulos.",
      "No extraer información académica extensa.",
      "No convertir Objetivo ni Presentación automáticamente en Descripción.",
      "Si no existe una descripción breve adecuada, eliminar el bloque.",
      "No inventar una descripción.",
      "Si un campo permitido no existe, eliminarlo.",
      "Los datos generales del footer no se consideran campos de contenido del programa."
    ]
  },

  "COORDINATOR_CONTROL": {
    "mandatory": true,
    "purpose": "Controlar correctamente la información de coordinadores o coordinadoras.",
    "rules": [
      "Si el PPTX contiene únicamente el nombre de un coordinador o coordinadora, puede utilizarse en un bloque 'MÁS INFORMACIÓN' o equivalente cuando el lienzo contemple ese bloque.",
      "Si solamente existe el nombre, solicitar al usuario el número de teléfono de esa persona antes de generar.",
      "No utilizar automáticamente el teléfono general de Dirección de Postgrado como teléfono del coordinador.",
      "No asumir que el teléfono institucional corresponde al coordinador.",
      "No inventar el teléfono del coordinador.",
      "Si el usuario proporciona el número, incorporarlo al bloque correspondiente.",
      "Si el usuario decide no proporcionar teléfono, eliminar el bloque de información del coordinador.",
      "El nombre del coordinador debe conservarse exactamente salvo corrección autorizada.",
      "No duplicar el nombre del coordinador en diferentes bloques."
    ],
    "required_question_when_only_name_exists": "El PPTX proporciona únicamente el nombre de la coordinadora. ¿Qué número de teléfono deseas colocar junto a su nombre en 'MÁS INFORMACIÓN'?"
  },

  "FOOTER_CONTROL": {
    "mandatory": true,
    "purpose": "Mantener el footer institucional del flyer maestro sin depender del PPTX para construirlo.",
    "footer_source_priority": "LIENZO / FLYER MAESTRO",
    "rules": [
      "Los datos institucionales generales del footer NO deben extraerse del PPTX para construir el footer.",
      "El footer del lienzo constituye la plantilla institucional de referencia.",
      "Conservar el footer institucional del lienzo y sus datos generales.",
      "El PPTX únicamente debe utilizarse para CORROBORAR que los datos del footer coinciden.",
      "La corroboración no convierte los datos del footer en contenido académico del nuevo programa.",
      "No reemplazar automáticamente los datos del footer por los datos encontrados en el PPTX.",
      "Si el PPTX y el footer del lienzo coinciden, continuar normalmente.",
      "Si existe una diferencia entre el PPTX y el footer del lienzo, informar la discrepancia antes de generar.",
      "No corregir automáticamente el footer por información del PPTX.",
      "No mover datos del footer hacia bloques superiores.",
      "No duplicar dirección, teléfono, Tele Fax, correo o web fuera del footer.",
      "No utilizar el teléfono general del footer como teléfono de coordinador salvo autorización expresa del usuario."
    ],
    "data_to_corrobate": [
      "Dirección",
      "Teléfono",
      "Tele Fax",
      "E-mail",
      "Sitio web"
    ],
    "current_reference_footer": {
      "Dirección": "Av. Arce s/n, Facultad de Minas",
      "Teléfono": "6227317 - 6228248",
      "Tele Fax": "2-6122467",
      "E-mail": "postgrado.uatf.potosi@gmail.com",
      "Web": "www.uatfpostgrado.edu.bo"
    },
    "important_rule": "Estos datos pertenecen al footer institucional y no deben volver a utilizarse como información del programa extraída del PPTX."
  },

  "EXCLUDED_CONTENT": {
    "mandatory": true,
    "excluded_fields": [
      "Objetivo",
      "Presentación como sección independiente",
      "Perfil de postulantes",
      "Perfil del posgraduado",
      "Criterios de admisión",
      "Requisitos de admisión",
      "Documentación requerida",
      "Plan de estudios",
      "Módulos",
      "Asignaturas",
      "Plataformas educativas",
      "Moodle",
      "Zoom",
      "Resoluciones",
      "Organización del curso",
      "Cronograma administrativo",
      "Fechas de publicación",
      "Fechas de registro",
      "Fechas de inscripción",
      "Actividades administrativas",
      "Información académica extensa",
      "Datos generales del footer como contenido del programa"
    ],
    "rule": "Aunque estos datos existan en el PPTX, no deben aparecer en el flyer."
  },

  "CORRECTION_CONTROL": {
    "mandatory": true,
    "uppercase_accents": {
      "automatic": true,
      "rule": "Corregir siempre las tildes faltantes en palabras completamente escritas en MAYÚSCULAS.",
      "examples": [
        "EDUCACION → EDUCACIÓN",
        "DIDACTICAS → DIDÁCTICAS",
        "PRACTICO → PRÁCTICO",
        "TITULACION → TITULACIÓN",
        "INFORMACION → INFORMACIÓN",
        "PUBLICA → PÚBLICA"
      ]
    },
    "word_corrections": {
      "automatic": false,
      "approval_required": true,
      "rule": "Si una corrección cambia una palabra, debe informarse antes de modificarla."
    },
    "protected_data": [
      "Nombres propios",
      "Nombres de programas",
      "Cifras",
      "Fechas",
      "Precios",
      "Nombres de personas",
      "Denominaciones institucionales"
    ],
    "critical_rule": "NINGUNA CORRECCIÓN QUE CAMBIE UNA PALABRA, NOMBRE, CIFRA, FECHA, PRECIO O SIGNIFICADO PUEDE APLICARSE SILENCIOSAMENTE."
  },

  "INCONSISTENCY_CONTROL": {
    "mandatory": true,
    "check": [
      "Fechas diferentes para el mismo evento",
      "Duraciones contradictorias",
      "Horarios contradictorios",
      "Precios diferentes",
      "Cargas horarias diferentes",
      "Créditos diferentes",
      "Nombres diferentes del mismo programa",
      "Modalidades diferentes",
      "Certificaciones diferentes",
      "Información institucional contradictoria"
    ],
    "rules": [
      "No elegir silenciosamente un valor sobre otro.",
      "No modificar datos contradictorios.",
      "Informar la inconsistencia.",
      "Solicitar decisión del usuario cuando afecte un dato del flyer.",
      "No utilizar información contradictoria hasta resolverla."
    ]
  },

  "DUPLICATION_AUDIT": {
    "mandatory": true,
    "instruction": "Auditar todo el contenido antes de generar para garantizar que ningún dato aparezca innecesariamente más de una vez.",
    "rules": [
      "No repetir tipo de programa.",
      "No repetir nombre del programa innecesariamente.",
      "No repetir modalidad.",
      "No repetir duración.",
      "No repetir titulación.",
      "No repetir horarios.",
      "No repetir fecha de inicio.",
      "No repetir inversión.",
      "No repetir inscripción.",
      "No repetir cuotas.",
      "No repetir coordinador.",
      "No repetir teléfono.",
      "No repetir dirección.",
      "No repetir correo.",
      "No repetir web.",
      "La información institucional completa pertenece al footer.",
      "Eliminar duplicaciones antes que llenar espacios vacíos."
    ]
  },

  "START_DATE": {
    "mandatory": true,
    "rules": [
      "La fecha de inicio debe tratarse como una única unidad visual.",
      "Día, mes y año deben utilizar el mismo color.",
      "La fecha completa debe aparecer en ROJO.",
      "No dividir la fecha entre colores.",
      "La fecha debe provenir del PPTX actual.",
      "Si no existe fecha válida, eliminar el bloque.",
      "Si existen fechas contradictorias, detener la generación y reportarlas."
    ]
  },

  "MAIN_IMAGE": {
    "mandatory": true,
    "instruction": "Crear o seleccionar una imagen principal relacionada exclusivamente con el programa actual.",
    "rules": [
      "La temática debe corresponder al programa actual.",
      "No reutilizar automáticamente imágenes anteriores.",
      "No introducir textos ficticios.",
      "No introducir logotipos ficticios.",
      "No introducir instituciones ficticias.",
      "No introducir información académica inexistente.",
      "Integrar la imagen profesionalmente con la composición del lienzo."
    ]
  },

  "INFORMATION_BLOCKS": {
    "mandatory": true,
    "allowed_blocks": [
      "Tipo de programa",
      "Nombre del programa",
      "Descripción breve",
      "Modalidad",
      "Duración",
      "Titulación o certificación",
      "Horas",
      "Créditos",
      "Número de plazas cuando corresponda",
      "Horarios",
      "Inicio",
      "Inversión",
      "Inscripción",
      "Cuotas",
      "Modalidad de pago",
      "Coordinador o coordinadora cuando corresponda",
      "Más información cuando corresponda",
      "Frase promocional cuando exista",
      "Footer institucional"
    ],
    "rules": [
      "Solo crear bloques con información válida.",
      "Si un campo no existe, eliminarlo.",
      "No crear bloques innecesarios.",
      "No utilizar textos de relleno.",
      "No utilizar POR DEFINIR.",
      "No utilizar PENDIENTE.",
      "No utilizar NO DISPONIBLE.",
      "No utilizar NO ESPECIFICADO.",
      "No utilizar POR CONFIRMAR.",
      "No utilizar A DEFINIR."
    ]
  },

  "PPTX_ISOLATION": {
    "mandatory": true,
    "source_priority": "PPTX ACTUAL",
    "rules": [
      "Cada PPTX es un proyecto independiente.",
      "No reutilizar fechas anteriores.",
      "No reutilizar precios anteriores.",
      "No reutilizar docentes o coordinadores anteriores.",
      "No reutilizar teléfonos anteriores como datos del programa.",
      "No reutilizar fotografías anteriores.",
      "No utilizar información de otros proyectos.",
      "No completar información mediante memoria.",
      "No completar información mediante otros PPTX."
    ]
  },

  "MISSING_INFORMATION": {
    "mandatory": true,
    "rule": "Si un campo permitido no existe en el PPTX, eliminarlo del diseño y redistribuir el espacio.",
    "forbidden_text": [
      "POR DEFINIR",
      "PENDIENTE",
      "NO DISPONIBLE",
      "NO ESPECIFICADO",
      "POR CONFIRMAR",
      "A DEFINIR"
    ]
  },

  "DESIGN_STYLE": {
    "mandatory": true,
    "style": [
      "Institucional",
      "Universitario",
      "Profesional",
      "Moderno",
      "Elegante",
      "Limpio",
      "Legible",
      "Alto impacto visual"
    ],
    "visual_rules": [
      "Mantener la estructura general del lienzo.",
      "Mantener la jerarquía visual.",
      "Mantener márgenes adecuados.",
      "Mantener equilibrio entre texto e imagen.",
      "Utilizar azul institucional, rojo institucional y blanco.",
      "No deformar escudos.",
      "No deformar fotografías.",
      "No superponer textos.",
      "No cortar palabras incorrectamente.",
      "No saturar de información.",
      "No convertir el PPTX completo en un flyer.",
      "Priorizar lectura rápida.",
      "No llenar espacios con información repetida.",
      "Respetar obligatoriamente la relación de aspecto 3:4."
    ]
  },

  "PRE_GENERATION_REPORT": {
    "mandatory": true,
    "instruction": "Antes de generar la imagen, mostrar qué información será utilizada, qué correcciones existen, qué inconsistencias existen, qué escudos serán incorporados y qué autorizaciones están pendientes.",
    "required_sections": [
      "INFORMACIÓN EXTRAÍDA DEL PPTX QUE SERÁ UTILIZADA",
      "TÍTULO Y NUMERACIÓN PROPUESTA",
      "AUTORIZACIÓN DE NUMERACIÓN",
      "DISTRIBUCIÓN DE DATOS",
      "CORRECCIONES PROPUESTAS",
      "INCONSISTENCIAS DETECTADAS",
      "CONTROL DEL FOOTER",
      "CONTROL DE COORDINADOR",
      "INFORMACIÓN EXCLUIDA",
      "CONTROL DE DUPLICACIONES",
      "ESCUDOS QUE SERÁN INCORPORADOS",
      "CONFIRMACIÓN PREVIA A GENERACIÓN"
    ],
    "critical_rule": "NO GENERAR HASTA RESOLVER TODAS LAS AUTORIZACIONES Y VALIDACIONES PENDIENTES."
  },

  "FINAL_VALIDATION": {
    "mandatory": true,
    "critical": true,
    "checklist": [
      "¿Se recibió el lienzo?",
      "¿Se recibió el PPTX actual?",
      "¿El lienzo fue utilizado como referencia visual?",
      "¿Se identificaron los campos del lienzo?",
      "¿Se identificaron exactamente los 3 escudos base?",
      "¿Se confirmó si existen escudos adicionales?",
      "¿Se informó el total exacto de escudos?",
      "¿El tipo de programa fue detectado automáticamente?",
      "¿El nombre oficial procede del PPTX?",
      "¿Se verificó la existencia de numeración romana?",
      "¿Si no existía numeración, se solicitó autorización para agregar I?",
      "¿La numeración utilizada fue autorizada?",
      "¿Se utilizaron únicamente campos autorizados?",
      "¿Se excluyeron Objetivo, Presentación, Perfil, Requisitos, Documentación, Plan de Estudios y Módulos?",
      "¿Se excluyeron Moodle, Zoom y Resoluciones?",
      "¿El footer fue tomado del lienzo y no construido desde el PPTX?",
      "¿El footer fue corroborado contra el PPTX?",
      "¿Se reportó cualquier discrepancia del footer?",
      "¿Si solo existe nombre de coordinador, se solicitó su teléfono?",
      "¿No se utilizó el teléfono general como teléfono del coordinador sin autorización?",
      "¿Se corrigieron automáticamente las tildes de MAYÚSCULAS?",
      "¿Se aprobaron las correcciones de palabras?",
      "¿Se resolvieron las inconsistencias?",
      "¿Se realizó auditoría de duplicaciones?",
      "¿La fecha completa está en rojo?",
      "¿No existe información inventada?",
      "¿No existe información POR DEFINIR o equivalente?",
      "¿La composición respeta el lienzo?",
      "¿El flyer tiene relación de aspecto 3:4?",
      "¿El resultado parece un flyer terminado y profesional?"
    ],
    "critical_failure_rule": "Si alguna respuesta es negativa, NO GENERAR. Corregir, consultar o detener el proceso."
  },

  "ABSOLUTE_RULES": [
    "EL LIENZO DEFINE LOS CAMPOS; EL PPTX DEFINE LOS VALORES.",
    "EL FOOTER DEL LIENZO DEFINE LOS DATOS INSTITUCIONALES GENERALES DEL FOOTER.",
    "EL PPTX SOLO CORROBORA LOS DATOS DEL FOOTER; NO LOS DEFINE.",
    "SI EL FOOTER DEL LIENZO Y EL PPTX DIFIEREN, INFORMAR LA DIFERENCIA Y NO CAMBIAR SILENCIOSAMENTE EL FOOTER.",
    "SI EL NOMBRE DEL PROGRAMA NO TIENE NUMERACIÓN ROMANA, PROPONER I PERO PREGUNTAR Y SOLICITAR AUTORIZACIÓN ANTES DE GENERAR.",
    "SI EL USUARIO PROPORCIONA II, III, IV, XVI U OTRA NUMERACIÓN, UTILIZAR EXACTAMENTE ESA NUMERACIÓN.",
    "NO INVENTAR NUMERACIONES.",
    "SI EL PPTX SOLO CONTIENE EL NOMBRE DEL COORDINADOR O COORDINADORA, PUEDE PROPONERSE UN BLOQUE MÁS INFORMACIÓN, PERO DEBE SOLICITARSE EL NÚMERO TELEFÓNICO ANTES DE GENERAR.",
    "NO UTILIZAR EL TELÉFONO GENERAL DEL FOOTER COMO TELÉFONO DEL COORDINADOR SIN AUTORIZACIÓN.",
    "NO DUPLICAR INFORMACIÓN DEL FOOTER EN BLOQUES SUPERIORES.",
    "NO GENERAR SIN MOSTRAR PREVIAMENTE LA INFORMACIÓN QUE SERÁ UTILIZADA.",
    "NO GENERAR SI EXISTE UNA CORRECCIÓN DE PALABRA PENDIENTE.",
    "NO GENERAR SI EXISTE UNA INCONSISTENCIA CRÍTICA NO RESUELTA.",
    "NO GENERAR SIN AUDITORÍA DE DUPLICACIONES.",
    "NO GENERAR SIN INFORMAR EL TOTAL EXACTO DE ESCUDOS.",
    "NO GENERAR UN CUARTO ESCUDO SIN AUTORIZACIÓN.",
    "LAS TILDES FALTANTES EN MAYÚSCULAS SIEMPRE DEBEN CORREGIRSE.",
    "LAS CORRECCIONES QUE CAMBIEN PALABRAS DEBEN MOSTRARSE ANTES DE APLICARSE.",
    "NO CAMBIAR NOMBRES PROPIOS, NOMBRES DE PROGRAMAS, CIFRAS, FECHAS, PRECIOS O DENOMINACIONES INSTITUCIONALES SIN AUTORIZACIÓN.",
    "NO UTILIZAR OBJETIVOS, PRESENTACIONES, PERFILES, REQUISITOS, PLANES DE ESTUDIO O MÓDULOS SIMPLEMENTE PORQUE EXISTAN EN EL PPTX.",
    "SI UN CAMPO NO TIENE VALOR VÁLIDO, ELIMINARLO.",
    "NO MOSTRAR POR DEFINIR, PENDIENTE, NO DISPONIBLE, NO ESPECIFICADO, POR CONFIRMAR NI A DEFINIR.",
    "SI EXISTE MENOS INFORMACIÓN, EL DISEÑO DEBE ADAPTARSE A ESA CANTIDAD.",
    "NO GENERAR CONTENIDO PARA LLENAR ESPACIOS.",
    "LA FECHA DE INICIO COMPLETA DEBE SER ROJA.",
    "EL FORMATO FINAL DEBE SER OBLIGATORIAMENTE 3:4.",
    "NO GENERAR HASTA SUPERAR TODAS LAS REGLAS CRÍTICAS."
  ]
}

# MÁS INFORMACIÓN

{
  "prompt": "Create ONLY a premium cinematic background image for a postgraduate academic program. The ONLY variable input is the postgraduate program name: {{POSTGRADUATE_PROGRAM_NAME}}.\n\nDISCIPLINE INTELLIGENCE:\nFirst, identify and understand the exact academic discipline, profession, specialization, scientific field or professional sector represented by the postgraduate program name. Do NOT rely only on predefined examples. The program may belong to ANY academic or professional field, including but not limited to engineering, medicine, nursing, veterinary medicine, dentistry, law, education, psychology, economics, finance, business, administration, architecture, design, communication, journalism, information technology, computer science, cybersecurity, data science, mathematics, physics, chemistry, biology, environmental sciences, agriculture, forestry, geology, social sciences, political science, international relations, humanities, languages, arts, tourism, hospitality, gastronomy, logistics, public administration, public health, laboratory sciences, pharmaceutical sciences, biomedical sciences, and any other specialized or emerging field.\n\nThe system must intelligently determine the profession and select the MOST AUTHENTIC professional objects, instruments, materials, technology and working environment for that specific postgraduate program.\n\nNEVER force a generic template onto different disciplines.\nNEVER use the same objects for every profession.\nNEVER add objects simply because they are associated with universities in general.\nThe visual concept must be specifically designed from the meaning of the postgraduate program name.\n\nCORE VISUAL CONCEPT:\nCreate ONE coherent, realistic professional environment photographed from very close range.\n\nThis is a PREMIUM CLOSE-UP EDITORIAL PHOTOGRAPH, NOT A LANDSCAPE.\n\nThe image should communicate the profession primarily through REAL PROFESSIONAL OBJECTS in the immediate foreground.\n\nThe most important discipline-specific objects must occupy approximately 65–75% of the composition and be large, sharp, highly detailed and immediately recognizable.\n\nSelect approximately 3–5 hero objects that are genuinely used by professionals or researchers in that field.\n\nExamples are ONLY references for reasoning, NOT a fixed list:\n\nEngineering may use helmets, laptops, plans, surveying equipment, structural materials and precision instruments.\nMedicine may use authentic medical instruments, diagnostic equipment, clinical materials and a medical workstation.\nNursing may use nursing instruments, clinical supplies, monitoring equipment and patient-care materials.\nVeterinary medicine may use veterinary diagnostic instruments, examination equipment and animal-care materials.\nDentistry may use authentic dental instruments, dental equipment and clinical materials.\nLaw may use legal books with no readable text, professional documents with no readable text, folders, legal workstation objects and appropriate technology.\nEducation may use pedagogical materials, teaching technology, educational research materials and an academic workstation.\nArchitecture may use physical architectural models, drafting instruments, material samples, plans and design technology.\nBusiness and finance may use professional laptops, financial analysis materials, calculators, documents without readable text and analytical technology.\nComputer science and information technology may use professional hardware, workstation equipment and realistic software/data visualization without readable text.\nLaboratory sciences may use authentic laboratory instruments, glassware, samples, microscopes and scientific equipment.\nCommunication and journalism may use cameras, microphones, professional recording equipment, editing technology and media-production tools.\nGastronomy may use professional culinary equipment, knives, cookware, ingredients and a realistic professional kitchen workstation.\nTourism and hospitality may use professional planning materials, travel-management technology and appropriate hospitality objects.\nEnvironmental sciences may use authentic field-research equipment, samples, scientific instruments and laboratory materials.\nAgricultural sciences may use agricultural research instruments, soil samples, crop-analysis equipment and professional field-research materials.\nSocial sciences may use research materials, analytical technology, field-research tools, documents without readable text and professional academic equipment.\nArts and design may use authentic creative tools, materials, professional equipment and appropriate studio objects.\n\nFor EVERY OTHER FIELD NOT LISTED ABOVE, independently determine the most recognizable and professionally authentic objects associated with that discipline.\n\nThe examples must NEVER limit the system's creativity or interpretation.\n\nFOREGROUND PRIORITY:\nThe camera must be positioned very close to the professional workstation, laboratory bench, clinical station, studio table, legal desk, engineering table, research station, kitchen station or equivalent professional workspace appropriate to the discipline.\n\nThe viewer should immediately see the professional objects before seeing the surrounding environment.\n\nThe hero objects must be physically present, correctly positioned and naturally interacting with the surface beneath them.\n\nEvery object must have realistic contact shadows, correct scale, correct perspective and physically accurate lighting.\n\nBACKGROUND:\nCreate only a subtle secondary environment that naturally belongs to the same profession.\n\nThe background should be darker, softer and slightly out of focus.\n\nIt may contain a laboratory, clinic, engineering facility, courtroom-inspired office, classroom, studio, research center, professional office, workshop, hospital environment, veterinary clinic, culinary kitchen, technology laboratory or any other authentic environment determined by the postgraduate discipline.\n\nThe background is SUPPORTING CONTEXT ONLY.\n\nDO NOT make the background the protagonist.\nDO NOT create a giant landscape.\nDO NOT create a huge sky.\nDO NOT create an ocean panorama.\nDO NOT create an aerial view.\nDO NOT create distant architecture as the main subject.\nDO NOT create a generic university campus.\n\nONE REAL LOCATION:\nEverything visible must logically exist in the same physical location and at the same moment.\n\nNo collages.\nNo split-screen compositions.\nNo floating objects.\nNo superimposed objects.\nNo unrelated environments.\nNo conceptual objects placed randomly in the scene.\n\nDocuments must physically rest on an appropriate surface.\nProfessional instruments must be located where professionals would actually use them.\nTechnology must be physically integrated into the environment.\nEquipment must be authentic to the discipline.\n\nVISUAL STYLE:\n- Square 1:1 composition\n- Ultra-high resolution\n- 4K quality\n- Photorealistic premium commercial photography\n- Sophisticated postgraduate university advertising aesthetic\n- Dark navy and charcoal shadows\n- Deep cyan-blue ambient illumination\n- Elegant warm gold and amber highlights\n- Consistent blue-and-gold cinematic color identity\n- High dynamic range\n- Realistic reflections\n- Physically accurate shadows\n- Extremely detailed materials\n- Premium shallow depth of field\n- Cinematic bokeh\n- Sophisticated color grading\n- Strong foreground separation\n- High-end editorial photography\n\nLIGHTING:\nUse the same premium BLUE + CYAN + GOLD + AMBER cinematic lighting language for every discipline.\n\nCool cyan-blue illumination should define shadows and background depth.\nWarm gold and amber highlights should emphasize the hero professional objects.\n\nThe lighting must adapt naturally to the environment. A hospital, laboratory, courtroom, engineering workstation, kitchen, studio or classroom should still look physically believable while maintaining the same overall blue-and-gold visual identity.\n\nAvoid excessive neon.\nAvoid science-fiction lighting.\nAvoid artificial glowing objects.\n\nMICRO-DETAILS:\nCreate extremely realistic surface details appropriate to the selected profession: paper fibers, subtle scratches, brushed metal, glass reflections, fabric, leather, plastic, wood, concrete, steel, medical instruments, laboratory glassware, computer hardware, architectural materials, culinary materials, scientific samples or any other discipline-specific material.\n\nREALISM:\nEvery object must be professionally authentic and physically believable.\n\nCorrect proportions.\nCorrect scale.\nCorrect perspective.\nCorrect materials.\nCorrect professional usage.\nCorrect contact shadows.\nCorrect reflections.\nCorrect environmental interaction.\nCorrect lighting.\n\nIf specialized instruments are shown, they must resemble REAL professional equipment rather than generic fictional objects.\n\nPEOPLE:\nDo not include people unless they genuinely strengthen the concept. If a person is necessary, show them naturally working within the professional environment rather than posing for the camera.\n\nThe person's face must not become the primary visual subject unless the academic discipline specifically requires it.\n\nTEXT-SAFE AREA:\nReserve approximately 25–35% of the composition for future typography.\n\nCreate natural negative space using darker surfaces, controlled shadows, soft blur, atmospheric depth or uncluttered parts of the professional environment.\n\nDo NOT create an artificial blank rectangle.\nDo NOT create a white empty area.\nDo NOT add a digital overlay.\nDo NOT sacrifice the professional objects merely to create empty space.\n\nThe future title must be able to sit naturally over this area.\n\nSTRICTLY FORBIDDEN:\n- Any readable text\n- Letters\n- Numbers\n- Words\n- Titles\n- Captions\n- Logos\n- Watermarks\n- Brand names\n- Readable screens\n- Readable documents\n- Readable book titles\n- Fake interface text\n- Random symbols resembling typography\n- Generic stock photography\n- Generic professional objects unrelated to the program\n- Collages\n- Split-screen layouts\n- Floating objects\n- Floating documents\n- Impossible environments\n- Objects from unrelated professions\n- Giant landscapes\n- Giant skies\n- Ocean-dominated scenes\n- Wide aerial views\n- Futuristic science-fiction objects\n- Excessive neon\n- Excessive particles\n- Cartoon aesthetics\n- Illustration aesthetics\n- Cheap 3D-render appearance\n- Videogame aesthetics\n- Artificial-looking objects\n- Deformed equipment\n- Duplicate objects\n- Impossible anatomy\n- Unrealistic professional instruments\n\nACADEMIC LEVEL:\nInterpret the level indicated by the program name.\n\nFor DOCTORATE and POSTDOCTORATE programs, communicate advanced research, intellectual depth, precision, innovation, specialized technology and prestige.\nFor MASTER'S programs, communicate advanced professional specialization, expertise and leadership.\nFor DIPLOMA or SPECIALIZATION programs, communicate practical professional specialization and technical expertise.\nFor BACHELOR'S or LICENTIATE programs, communicate professional formation, academic development and contemporary knowledge.\n\nFINAL DECISION PROCESS:\nBefore generating the image, internally determine:\n1. What profession or scientific field does the program represent?\n2. What 3–5 objects would immediately identify that profession?\n3. What professional environment naturally contains those objects?\n4. Which object should be the main hero?\n5. Where should the text-safe area be placed?\n6. How can the blue-and-gold cinematic lighting enhance those objects?\n\nThen generate ONE coherent photograph based on those decisions.\n\nMOST IMPORTANT RULE:\nTHE POSTGRADUATE PROGRAM NAME IS THE SOURCE OF TRUTH.\nDO NOT LIMIT THE VISUAL CONCEPT TO THE EXAMPLES PROVIDED IN THIS PROMPT.\nIF THE PROGRAM BELONGS TO AN AREA NOT EXPLICITLY MENTIONED, IDENTIFY THAT AREA AND CREATE THE CORRECT PROFESSIONAL VISUAL LANGUAGE AUTOMATICALLY.\n\nPrioritize authentic foreground objects over scenery.\nPrioritize professional relevance over decorative complexity.\nPrioritize physical coherence over conceptual effects.\nPrioritize photorealism over spectacle.\n\nThe final image must immediately communicate the specific academic field while maintaining a prestigious, sophisticated and consistent postgraduate campaign aesthetic.\n\nGenerate ONLY the clean photographic background. No text, no logos and no graphic design elements.",
  "input": {
    "POSTGRADUATE_PROGRAM_NAME": "Enter only the postgraduate program name"
  },
  "output": {
    "type": "premium_cinematic_academic_background",
    "aspect_ratio": "1:1",
    "resolution": "4K",
    "photorealistic": true,
    "cinematic": true,
    "color_style": "deep navy, cyan blue, gold and amber",
    "camera_style": "close-up professional editorial photography",
    "foreground_priority": "extreme",
    "discipline_adaptation": "fully automatic",
    "professional_object_selection": "automatic",
    "environment_selection": "automatic",
    "academic_level_adaptation": "automatic",
    "text_in_image": false,
    "logos": false,
    "watermarks": false,
    "typography": false,
    "single_environment": true,
    "physical_coherence": true
  }
}

# 
# FLYERS

{
  "prompt_name": "PROMPT_MAESTRO_FINAL_FLYER_UATF_LIENZO_PPTX",
  "version": "FINAL_V6_CONTROL_TOTAL_3_4_BLOQUES_HEADERS_PROTEGIDOS",
  "purpose": "Crear flyers institucionales profesionales de la Universidad Autónoma Tomás Frías utilizando una IMAGEN DE LIENZO como referencia maestra de estructura visual y un PPTX ACTUAL como fuente de contenido. El lienzo define los campos, jerarquía, composición, bloques, headers, geometrías y diseño visual. El PPTX define exclusivamente los valores reales de los campos académicos, administrativos y financieros del programa.",
  
  "FORMAT": {
    "aspect_ratio": "3:4",
    "orientation": "vertical",
    "mandatory": true,
    "rule": "El flyer final debe generarse obligatoriamente en relación de aspecto 3:4.",
    "priority": "No deformar, recortar incorrectamente ni alterar la estructura visual del lienzo para adaptar el contenido al formato 3:4."
  },

  "CORE_PRINCIPLE": {
    "rule": "EL LIENZO DEFINE QUÉ CAMPOS, BLOQUES Y ELEMENTOS VISUALES DEBEN EXISTIR, CÓMO SE ORGANIZAN Y CÓMO SE PRESENTAN. EL PPTX DEFINE LOS VALORES REALES QUE DEBEN COLOCARSE DENTRO DE ESOS ELEMENTOS.",
    "absolute_rules": [
      "No reutilizar contenido académico de otros proyectos.",
      "No inventar información.",
      "No completar datos faltantes con conocimientos externos.",
      "No trasladar automáticamente información del lienzo al nuevo proyecto como contenido académico.",
      "El lienzo es referencia visual, estructural y de campos; nunca es fuente de contenido académico del nuevo programa.",
      "La existencia de un dato en el PPTX no significa que deba aparecer en el flyer.",
      "Si un campo permitido no existe en el PPTX, no inventar su contenido.",
      "Los elementos visuales protegidos del lienzo no deben eliminarse únicamente porque un campo de contenido esté ausente.",
      "Nunca utilizar textos de relleno.",
      "Nunca corregir silenciosamente palabras del PPTX.",
      "Las tildes faltantes en palabras completamente escritas en MAYÚSCULAS deben corregirse automáticamente.",
      "Toda corrección que cambie una palabra, nombre, cifra, fecha, precio o significado debe ser informada y aprobada antes de aplicarse.",
      "No generar la imagen mientras exista información pendiente de revisión, inconsistencia no resuelta o corrección que requiera aprobación."
    ]
  },

  "WORKFLOW": {
    "mandatory_order": [
      "Recibir IMAGEN DE LIENZO.",
      "Recibir PPTX ACTUAL.",
      "Analizar el lienzo para identificar estructura, jerarquía, composición, campos, bloques y diseño visual.",
      "Identificar los 3 escudos base.",
      "Preguntar si se desean escudos adicionales.",
      "Validar los escudos adicionales proporcionados directamente por el usuario.",
      "Analizar el PPTX actual.",
      "Detectar automáticamente el tipo de programa.",
      "Detectar automáticamente el nombre oficial del programa.",
      "Detectar si el nombre oficial contiene numeral romano.",
      "Si falta numeral romano, solicitar autorización antes de agregarlo.",
      "Buscar únicamente los campos definidos por el lienzo.",
      "Identificar cuáles bloques visuales son permanentes y cuáles son condicionales.",
      "Excluir información no autorizada.",
      "Corroborar el footer institucional del lienzo contra el PPTX sin reemplazarlo automáticamente.",
      "Detectar tildes faltantes.",
      "Corregir automáticamente únicamente tildes faltantes en MAYÚSCULAS.",
      "Reportar y solicitar aprobación para correcciones que cambien palabras o significado.",
      "Detectar inconsistencias internas.",
      "Detectar información de coordinadora.",
      "Si existe nombre de coordinadora pero no teléfono, solicitar el número antes de generar.",
      "Elaborar reporte previo.",
      "Realizar auditoría global de duplicaciones.",
      "Verificar expresamente la conservación de los bloques visuales protegidos.",
      "Informar el total exacto de escudos.",
      "Realizar validación previa a generación.",
      "Generar únicamente después de superar todas las validaciones.",
      "Validar el flyer final."
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
    "instruction": "Analizar el lienzo para determinar estructura visual, jerarquía, composición, distribución espacial, campos informativos, bloques permanentes, bloques condicionales y lenguaje visual.",
    "preserve": [
      "Formato",
      "Orientación",
      "Proporciones",
      "Márgenes",
      "Header institucional",
      "Distribución de escudos",
      "Jerarquía tipográfica",
      "Tipo de programa",
      "Nombre del programa",
      "Descripción breve",
      "Área de imagen principal",
      "Bloques de información académica",
      "Headers de cada bloque",
      "Bloque de inicio",
      "Bloques financieros",
      "Bloque de más información",
      "Bloque de reducción de costos",
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
      "Nunca copiar teléfonos del lienzo.",
      "Nunca copiar docentes del lienzo.",
      "Nunca utilizar información académica del lienzo como dato del nuevo proyecto.",
      "El lienzo determina qué información buscar y cómo presentarla visualmente.",
      "Los elementos visuales permanentes del lienzo deben conservarse aunque el PPTX no contenga datos para completar su contenido."
    ]
  },

  "HEADER_DESIGN_LOCK": {
    "mandatory": true,
    "critical": true,
    "purpose": "Impedir que el generador rediseñe, sustituya, elimine o interprete libremente los encabezados de los bloques del lienzo.",
    "protected_headers": [
      "MODALIDAD",
      "DURACIÓN",
      "TITULACIÓN",
      "NÚMERO DE PLAZAS",
      "HORARIOS",
      "INICIO DE ESTUDIOS",
      "INVERSIÓN",
      "MODALIDAD DE PAGO",
      "MÁS INFORMACIÓN",
      "REDUCCIÓN EN LOS COSTOS DE TITULACIÓN"
    ],
    "rule": "Los headers anteriores son ELEMENTOS VISUALES PROTEGIDOS DEL LIENZO. Deben conservar exactamente la lógica visual, forma, posición, proporción, color y jerarquía del lienzo de referencia.",
    "protected_properties": [
      "Forma",
      "Geometría",
      "Color",
      "Tipografía",
      "Peso tipográfico",
      "Tamaño relativo",
      "Altura",
      "Ancho",
      "Proporción",
      "Posición",
      "Alineación",
      "Bordes",
      "Grosor de bordes",
      "Radio de esquinas",
      "Fondo",
      "Separación",
      "Margen interno",
      "Jerarquía",
      "Estilo de cápsula o rectángulo cuando exista",
      "Relación con el icono asociado",
      "Relación con el contenido inferior"
    ],
    "strict_rules": [
      "NO rediseñar los headers.",
      "NO crear un nuevo estilo de header.",
      "NO convertir rectángulos en cápsulas.",
      "NO convertir cápsulas en rectángulos.",
      "NO cambiar colores de los headers.",
      "NO intercambiar azul y rojo.",
      "NO eliminar bordes existentes.",
      "NO agregar bordes inexistentes.",
      "NO cambiar la tipografía visual del header.",
      "NO cambiar el tamaño relativo del header.",
      "NO cambiar la posición del header.",
      "NO cambiar la alineación.",
      "NO agregar sombras si el lienzo no las tiene.",
      "NO eliminar sombras si el lienzo las tiene.",
      "NO alterar la forma para llenar espacio.",
      "NO sustituir el diseño por botones genéricos.",
      "NO reinterpretar el header según el contenido del PPTX.",
      "El PPTX solamente determina el texto o valor que debe colocarse dentro del bloque.",
      "El diseño del header pertenece al lienzo y debe permanecer protegido."
    ],
    "priority": "DISEÑO DEL HEADER DEL LIENZO > INTERPRETACIÓN LIBRE DEL GENERADOR",
    "critical_rule": "Si existe diferencia entre el diseño del header generado y el header del lienzo, debe considerarse un error de generación y corregirse."
  },

  "REDUCTION_COSTS_BLOCK_LOCK": {
    "mandatory": true,
    "critical": true,
    "purpose": "Garantizar que el cuadro visual azul correspondiente a REDUCCIÓN EN LOS COSTOS DE TITULACIÓN permanezca siempre presente y conserve exactamente la estructura del lienzo de referencia.",
    
    "protected_block_name": "REDUCCIÓN EN LOS COSTOS DE TITULACIÓN",
    
    "permanent_visual_element": true,
    
    "critical_rule": "EL CUADRO AZUL DE REDUCCIÓN EN LOS COSTOS DE TITULACIÓN ES UN ELEMENTO VISUAL PERMANENTE DEL LIENZO Y DEBE MANTENERSE SIEMPRE. NUNCA DEBE ELIMINARSE, SUSTITUIRSE, CAMBIARSE DE POSICIÓN NI REDISEÑARSE POR EL HECHO DE QUE EL PPTX NO CONTENGA INFORMACIÓN DE REDUCCIÓN DE COSTOS.",
    
    "protected_elements": [
      "Cuadro azul completo",
      "Header REDUCCIÓN EN LOS COSTOS DE TITULACIÓN",
      "Forma geométrica del cuadro",
      "Color azul institucional",
      "Bordes",
      "Proporciones",
      "Altura",
      "Ancho",
      "Posición",
      "Alineación",
      "Icono asociado cuando exista",
      "Tipografía del header",
      "Jerarquía visual",
      "Decoraciones gráficas",
      "Elementos diagonales o laterales cuando existan",
      "Relación con el resto de bloques del lienzo"
    ],
    
    "mandatory_rules": [
      "SIEMPRE mantener el cuadro azul de REDUCCIÓN EN LOS COSTOS DE TITULACIÓN.",
      "SIEMPRE mantener visible el header REDUCCIÓN EN LOS COSTOS DE TITULACIÓN.",
      "NO eliminar el cuadro aunque el PPTX no contenga información sobre reducción de costos.",
      "NO sustituir el cuadro por otro bloque.",
      "NO cambiar el cuadro azul por otro color.",
      "NO cambiar el cuadro azul a rojo.",
      "NO eliminar el header.",
      "NO convertir el cuadro en una cápsula.",
      "NO convertir el cuadro en un rectángulo diferente al del lienzo.",
      "NO modificar su geometría.",
      "NO modificar su posición.",
      "NO modificar sus proporciones.",
      "NO eliminar el icono asociado cuando forme parte del diseño del lienzo.",
      "NO rellenar el cuadro con información de otro campo.",
      "NO utilizar información de reducción proveniente de proyectos anteriores.",
      "NO inventar porcentajes, descuentos, montos ni beneficios.",
      "NO copiar automáticamente el texto promocional de reducción que aparezca en el lienzo.",
      "El contenido interno del cuadro solamente puede provenir del PPTX ACTUAL o de una autorización explícita del usuario.",
      "Si el PPTX no contiene información de reducción, mantener el cuadro y su header como estructura gráfica, pero no inventar contenido.",
      "El cuadro debe conservar su presencia visual aunque su área interna de contenido quede vacía o sea adaptada visualmente sin alterar su estructura.",
      "Nunca eliminar este bloque para ganar espacio para otros contenidos.",
      "Nunca redistribuir este bloque como si fuera un bloque condicional.",
      "Este bloque tiene prioridad estructural sobre cualquier intento de compactar o reorganizar el flyer."
    ],
    
    "content_rule": {
      "source": "PPTX_ACTUAL",
      "rule": "El PPTX determina únicamente el contenido interno del cuadro. El lienzo determina obligatoriamente la existencia, estructura, diseño y apariencia del cuadro.",
      "if_content_exists": "Colocar únicamente la información de reducción de costos realmente encontrada en el PPTX.",
      "if_content_does_not_exist": "Mantener el cuadro azul y su header exactamente como en el lienzo, sin inventar información y sin sustituirlo por otro contenido.",
      "if_content_conflicts": "Detener la generación y reportar la inconsistencia."
    },
    
    "priority": "EXISTENCIA Y DISEÑO DEL CUADRO > DISPONIBILIDAD DE CONTENIDO EN EL PPTX",
    
    "validation": [
      "¿El cuadro azul de REDUCCIÓN EN LOS COSTOS DE TITULACIÓN permanece visible?",
      "¿El header mantiene exactamente su diseño?",
      "¿El cuadro mantiene su color azul?",
      "¿El cuadro mantiene su posición y proporción?",
      "¿Se evitó eliminarlo por falta de datos?",
      "¿Se evitó inventar información?",
      "¿El contenido, si existe, procede exclusivamente del PPTX actual?"
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
    "count_confirmation": {
      "formula": "TOTAL_ESCUDOS = 3 ESCUDOS BASE + ESCUDOS ADICIONALES APROBADOS",
      "mandatory_message": "ANTES DE GENERAR: incorporaré un total de [N] ESCUDOS: [lista exacta].",
      "default_message": "ANTES DE GENERAR: incorporaré un total de 3 ESCUDOS: UATF, Dirección de Postgrado UATF y CEUB.",
      "rules": [
        "No generar antes de informar el total.",
        "No agregar escudos que no hayan sido anunciados.",
        "No cambiar el número después de la confirmación."
      ]
    }
  },

  "ROMAN_NUMERAL_CONTROL": {
    "mandatory": true,
    "critical": true,
    "purpose": "Controlar el numeral romano del programa cuando el usuario maneja consecutivamente I, II, III, XVI, etc.",
    "rules": [
      "Detectar automáticamente si el nombre oficial del programa contiene numeral romano.",
      "Si el PPTX contiene un numeral romano, conservarlo exactamente.",
      "Ejemplos válidos: I, II, III, IV, V, VI, VII, VIII, IX, X, XI, XII, XIII, XIV, XV, XVI.",
      "Si el PPTX no contiene numeral romano, NO agregarlo automáticamente.",
      "Si el nombre aparece como 'DIPLOMADO EN...' sin numeral, informar al usuario que no se detectó numeral.",
      "Preguntar expresamente si desea agregar 'I' u otro numeral.",
      "No generar el flyer hasta obtener autorización cuando el numeral sea necesario.",
      "Una vez autorizado por el usuario, incorporar exactamente el numeral indicado.",
      "No inventar un numeral diferente.",
      "No reutilizar el numeral de otro proyecto."
    ],
    "required_question": "No se detecta numeral romano en el nombre del programa. ¿Deseas agregar I al inicio del título?",
    "example_authorized": {
      "input": "DIPLOMADO EN GESTIÓN Y ADMINISTRACIÓN PÚBLICA CON ENFOQUE NORMATIVO",
      "authorized_result": "I DIPLOMADO EN GESTIÓN Y ADMINISTRACIÓN PÚBLICA CON ENFOQUE NORMATIVO"
    }
  },

  "PROGRAM_TYPE_DETECTION": {
    "mandatory": true,
    "rules": [
      "Detectar automáticamente el tipo de programa a partir del nombre oficial del PPTX.",
      "No pedir al usuario el tipo cuando el PPTX lo identifica claramente.",
      "No inventar el tipo de programa.",
      "Utilizar la denominación oficial encontrada en el PPTX."
    ]
  },

  "TITLE_STRUCTURE": {
    "mandatory": true,
    "rules": [
      "Construir automáticamente la jerarquía visual del título.",
      "No modificar el significado del nombre oficial.",
      "No eliminar palabras importantes.",
      "La distribución de líneas debe priorizar legibilidad.",
      "El numeral romano autorizado debe formar parte del título.",
      "No mostrar instrucciones internas en el flyer.",
      "No escribir etiquetas como 'VERSIÓN DOCTORADO' o similares."
    ]
  },

  "ALLOWED_CONTENT_FIELDS": {
    "mandatory": true,
    "fields": {
      "program_identification": [
        "Tipo de programa",
        "Nombre oficial del programa"
      ],
      "main_description": [
        "Descripción o frase descriptiva principal"
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
        "Inicio del programa"
      ],
      "financial_information": [
        "Inversión",
        "Costo total",
        "Costo de colegiatura",
        "Monto de inscripción",
        "Cuotas",
        "Pagos mensuales",
        "Modalidad de pago",
        "Plan de pago",
        "Reducción de costos de titulación cuando exista"
      ],
      "complementary_information": [
        "Coordinador o coordinadora cuando corresponda",
        "Frase institucional o promocional cuando exista"
      ]
    },
    "rules": [
      "Solo buscar campos que correspondan a bloques existentes en el lienzo.",
      "No extraer Objetivo como campo independiente.",
      "No extraer Presentación como campo independiente.",
      "No extraer Perfil como campo independiente.",
      "No extraer Requisitos.",
      "No extraer Plan de Estudios.",
      "No extraer Módulos.",
      "No inventar descripción.",
      "La ausencia de un dato de contenido no autoriza a eliminar un elemento visual protegido.",
      "Si un campo permitido no existe, no inventar su contenido."
    ]
  },

  "COORDINATOR_CONTROL": {
    "mandatory": true,
    "rules": [
      "Buscar específicamente los campos COORDINADOR y COORDINADORA en el PPTX.",
      "Si aparece el nombre de una coordinadora y el lienzo posee un bloque MÁS INFORMACIÓN, el nombre puede colocarse allí.",
      "Si únicamente aparece el nombre y no existe teléfono asociado, solicitar el número telefónico al usuario antes de generar.",
      "No inventar un número telefónico.",
      "No utilizar números de proyectos anteriores.",
      "No generar el bloque de contacto de la coordinadora hasta disponer del número cuando este sea requerido por el diseño.",
      "El teléfono proporcionado por el usuario debe conservarse exactamente."
    ],
    "required_question_if_missing_phone": "Encontré el nombre de la coordinadora en el PPTX, pero no un número telefónico. ¿Qué número debo colocar en MÁS INFORMACIÓN?"
  },

  "FOOTER_VERIFICATION": {
    "mandatory": true,
    "purpose": "El footer institucional pertenece al lienzo de referencia y no debe depender de que esos datos aparezcan nuevamente en el PPTX.",
    "reference_footer": {
      "Direccion": "Av. Arce s/n, Facultad de Minas",
      "Telefono": "6227317 - 6228248",
      "Tele_Fax": "2-6122467",
      "E_mail": "postgrado.uatf.potosi@gmail.com",
      "Web": "www.uatfpostgrado.edu.bo"
    },
    "rules": [
      "No es necesario extraer estos datos del PPTX para construir el footer.",
      "El footer debe conservar la información institucional del lienzo de referencia.",
      "El PPTX puede utilizarse únicamente para corroborar que estos datos coinciden.",
      "Si coinciden, mantener el footer del lienzo.",
      "Si no coinciden, informar la diferencia antes de modificar cualquier dato.",
      "No reemplazar silenciosamente los datos del footer.",
      "No eliminar el footer porque el PPTX no contenga esos datos.",
      "No duplicar estos datos en bloques superiores."
    ]
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
      "Cualquier dato que no corresponda a un bloque autorizado"
    ],
    "rule": "Aunque un dato exista en el PPTX, no debe aparecer si está excluido o no corresponde a un bloque autorizado del lienzo."
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
        "INFORMACION → INFORMACIÓN"
      ]
    },
    "word_corrections": {
      "automatic": false,
      "approval_required": true,
      "rule": "Si una corrección cambia una palabra original, informar antes de modificarla."
    },
    "semantic_changes": {
      "automatic": false,
      "approval_required": true,
      "protected_data": [
        "Nombres propios",
        "Nombres de programas",
        "Cifras",
        "Fechas",
        "Precios",
        "Nombres de personas",
        "Denominaciones institucionales"
      ]
    }
  },

  "INCONSISTENCY_CONTROL": {
    "mandatory": true,
    "check": [
      "Fechas diferentes",
      "Duraciones contradictorias",
      "Horarios contradictorios",
      "Precios diferentes",
      "Cargas horarias diferentes",
      "Créditos diferentes",
      "Nombres diferentes del mismo programa",
      "Modalidades diferentes",
      "Certificaciones diferentes",
      "Información institucional contradictoria",
      "Información contradictoria sobre reducción de costos de titulación"
    ],
    "rules": [
      "No elegir silenciosamente un valor sobre otro.",
      "No modificar datos contradictorios.",
      "Informar la inconsistencia.",
      "Solicitar decisión del usuario cuando afecte un dato del flyer."
    ]
  },

  "DUPLICATION_AUDIT": {
    "mandatory": true,
    "instruction": "Auditar todo el contenido antes de generar para garantizar que ningún dato aparezca innecesariamente más de una vez.",
    "rules": [
      "Eliminar duplicaciones antes de llenar espacios.",
      "No repetir teléfono, WhatsApp, correo, web o dirección fuera del footer.",
      "No repetir fecha de inicio.",
      "No repetir modalidad.",
      "No repetir duración.",
      "No repetir inversión.",
      "No repetir inscripción.",
      "No repetir cuotas.",
      "No repetir coordinadora.",
      "No repetir frases descriptivas.",
      "No duplicar información de reducción de costos.",
      "NO eliminar bloques visuales protegidos para evitar duplicaciones.",
      "ELIMINAR DUPLICACIONES > LLENAR ESPACIO."
    ]
  },

  "START_DATE": {
    "mandatory": true,
    "format_rule": "La fecha debe mostrarse siempre con el día en número, seguido del mes escrito completamente en palabras y finalmente el año en números.",
    "format_example": "04 de septiembre de 2026",
    "rules": [
      "La fecha debe provenir exclusivamente del PPTX actual.",
      "No reutilizar fechas de otros proyectos.",
      "El diseño visual y color de la fecha deben seguir el lienzo de referencia.",
      "NO imponer que la fecha completa sea roja.",
      "NO imponer que día, mes y año tengan el mismo color.",
      "NO modificar los colores definidos por el lienzo.",
      "Si no existe fecha de inicio válida, mantener el bloque visual de INICIO DE ESTUDIOS, pero no inventar una fecha.",
      "Si existen fechas contradictorias, detener la generación y reportarlas."
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
      "Titulación",
      "Número de plazas",
      "Horarios",
      "Inicio de estudios",
      "Inversión",
      "Modalidad de pago",
      "Más información",
      "Reducción de costos de titulación",
      "Footer institucional"
    ],
    "permanent_visual_blocks": [
      "Reducción de costos de titulación"
    ],
    "rules": [
      "Los bloques deben seguir el diseño del lienzo.",
      "Los headers de los bloques están protegidos por HEADER_DESIGN_LOCK.",
      "El bloque REDUCCIÓN DE COSTOS DE TITULACIÓN está adicionalmente protegido por REDUCTION_COSTS_BLOCK_LOCK.",
      "Solo cambiar los valores de contenido provenientes del PPTX.",
      "No cambiar el diseño para adaptarlo al contenido.",
      "Si un campo no existe, no inventar contenido.",
      "Los bloques permanentes del lienzo NO deben eliminarse por ausencia de contenido.",
      "En bloques condicionales, si un campo no existe, eliminar únicamente el contenido y redistribuir el espacio sin rediseñar innecesariamente los headers restantes.",
      "El cuadro azul de REDUCCIÓN EN LOS COSTOS DE TITULACIÓN nunca debe eliminarse.",
      "No utilizar textos de relleno.",
      "No utilizar POR DEFINIR.",
      "No utilizar PENDIENTE.",
      "No utilizar NO DISPONIBLE.",
      "No utilizar NO ESPECIFICADO.",
      "No utilizar POR CONFIRMAR.",
      "No utilizar A DEFINIR."
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
      "Mantener los headers exactamente según HEADER_DESIGN_LOCK.",
      "Mantener el cuadro azul de REDUCCIÓN EN LOS COSTOS DE TITULACIÓN exactamente según REDUCTION_COSTS_BLOCK_LOCK.",
      "Mantener márgenes adecuados.",
      "Mantener equilibrio entre texto e imagen.",
      "Utilizar azul institucional, rojo institucional y blanco según el lienzo.",
      "No deformar escudos.",
      "No deformar fotografías.",
      "No superponer textos.",
      "No cortar palabras incorrectamente.",
      "No saturar de información.",
      "No llenar espacios con información repetida.",
      "No eliminar elementos visuales protegidos para ganar espacio.",
      "Respetar obligatoriamente la relación de aspecto 3:4."
    ]
  },

  "PRE_GENERATION_REPORT": {
    "mandatory": true,
    "required_sections": [
      "INFORMACIÓN EXTRAÍDA DEL PPTX QUE SERÁ UTILIZADA",
      "TIPO Y TÍTULO DETECTADOS",
      "NUMERAL ROMANO DETECTADO O PENDIENTE DE AUTORIZACIÓN",
      "DISTRIBUCIÓN DE LOS DATOS EN EL FLYER",
      "CORRECCIONES PROPUESTAS",
      "INCONSISTENCIAS DETECTADAS",
      "INFORMACIÓN EXCLUIDA",
      "CONTROL DEL FOOTER",
      "CONTROL DE DUPLICACIONES",
      "COORDINADORA Y TELÉFONO",
      "ESCUDOS QUE SERÁN INCORPORADOS",
      "CONTROL DEL CUADRO REDUCCIÓN EN LOS COSTOS DE TITULACIÓN",
      "CONFIRMACIÓN PREVIA A GENERACIÓN"
    ],
    "critical_rule": "NO GENERAR LA IMAGEN HASTA HABER PRESENTADO EL REPORTE Y RESUELTO TODA INFORMACIÓN QUE REQUIERA APROBACIÓN."
  },

  "FINAL_VALIDATION": {
    "mandatory": true,
    "critical": true,
    "checklist": [
      "¿Se recibió el lienzo?",
      "¿Se recibió el PPTX?",
      "¿El lienzo fue utilizado como referencia visual y de campos?",
      "¿Se identificaron exactamente los 3 escudos base?",
      "¿Se informó el total exacto de escudos?",
      "¿El tipo de programa procede del PPTX?",
      "¿El nombre oficial procede del PPTX?",
      "¿Se verificó el numeral romano?",
      "¿Se solicitó autorización si faltaba numeral?",
      "¿El título conserva el numeral autorizado?",
      "¿Se utilizaron únicamente campos autorizados?",
      "¿Se excluyeron Objetivo, Presentación, Perfil, Requisitos, Plan de Estudios y Módulos?",
      "¿Se excluyeron Moodle, Zoom y Resoluciones?",
      "¿Se verificó el footer institucional contra el PPTX?",
      "¿Se detectó coordinadora?",
      "¿Se solicitó teléfono cuando era necesario?",
      "¿Se mostraron las correcciones?",
      "¿Se corrigieron automáticamente las tildes de MAYÚSCULAS?",
      "¿Se resolvieron las inconsistencias?",
      "¿Se realizó auditoría de duplicaciones?",
      "¿Los headers mantienen exactamente el diseño del lienzo?",
      "¿No se rediseñaron MODALIDAD, DURACIÓN, TITULACIÓN, NÚMERO DE PLAZAS, HORARIOS, INICIO DE ESTUDIOS, INVERSIÓN, MODALIDAD DE PAGO ni MÁS INFORMACIÓN?",
      "¿El cuadro azul de REDUCCIÓN EN LOS COSTOS DE TITULACIÓN permanece visible?",
      "¿El header REDUCCIÓN EN LOS COSTOS DE TITULACIÓN mantiene exactamente su diseño?",
      "¿El cuadro de reducción conserva su color azul?",
      "¿El cuadro de reducción conserva su forma, posición, proporción, bordes e iconografía?",
      "¿El cuadro de reducción se mantuvo aunque el PPTX no contenga datos de reducción?",
      "¿No se inventó ningún porcentaje, descuento, monto o beneficio de reducción?",
      "¿Si existe información de reducción, procede exclusivamente del PPTX actual?",
      "¿La fecha conserva el tratamiento visual del lienzo?",
      "¿La fecha está escrita como día + mes en palabra + año numérico?",
      "¿No se impuso que la fecha sea completamente roja?",
      "¿No existe información inventada?",
      "¿No existe POR DEFINIR, PENDIENTE o equivalente?",
      "¿El flyer respeta 3:4?",
      "¿El resultado mantiene la estructura visual del lienzo?"
    ],
    "critical_failure_rule": "Si alguna respuesta es negativa, NO GENERAR. Corregir, consultar o detener el proceso según corresponda."
  },

  "ABSOLUTE_RULES": [
    "NO GENERAR SIN REPORTE PREVIO.",
    "NO GENERAR CON CORRECCIONES DE PALABRAS PENDIENTES.",
    "NO GENERAR CON INCONSISTENCIAS NO RESUELTAS.",
    "NO GENERAR SIN AUDITORÍA DE DUPLICACIONES.",
    "NO GENERAR SIN INFORMAR EL TOTAL EXACTO DE ESCUDOS.",
    "NO GENERAR UN CUARTO ESCUDO SIN AUTORIZACIÓN.",
    "NO AGREGAR NUMERAL ROMANO SI NO FUE AUTORIZADO.",
    "SI EL PPTX NO TIENE NUMERAL ROMANO, PREGUNTAR ANTES DE AGREGAR I.",
    "SI EL USUARIO AUTORIZA I, UTILIZAR I.",
    "SI EL USUARIO PROPORCIONA II, III, XVI U OTRO NUMERAL, CONSERVARLO EXACTAMENTE.",
    "NO EXTRAER EL FOOTER COMO CONTENIDO OBLIGATORIO DEL PPTX.",
    "EL FOOTER DEL LIENZO DEBE SER CORROBORADO, NO REEMPLAZADO SILENCIOSAMENTE.",
    "NO DUPLICAR INFORMACIÓN DEL FOOTER.",
    "NO REDISEÑAR LOS HEADERS DE LOS BLOQUES.",
    "LOS HEADERS DEL LIENZO SON ELEMENTOS VISUALES PROTEGIDOS.",
    "EL CONTENIDO DEL PPTX PUEDE CAMBIAR; EL DISEÑO DEL HEADER NO.",
    "NO CAMBIAR FORMA, COLOR, TIPOGRAFÍA, PROPORCIÓN, POSICIÓN NI ESTILO DE LOS HEADERS.",
    "NO IMPONER QUE LA FECHA SEA TOTALMENTE ROJA.",
    "LA FECHA DEBE SEGUIR LOS COLORES Y TRATAMIENTO VISUAL DEL LIENZO.",
    "LA FECHA DEBE MOSTRARSE COMO DÍA EN NÚMERO + MES ESCRITO EN PALABRA + AÑO EN NÚMERO.",
    "NO UTILIZAR INFORMACIÓN DE PROYECTOS ANTERIORES.",
    "NO INVENTAR INFORMACIÓN PARA LLENAR ESPACIOS.",
    "SI UN CAMPO NO EXISTE, NO INVENTAR SU CONTENIDO.",
    "NO ELIMINAR ELEMENTOS VISUALES PERMANENTES DEL LIENZO POR AUSENCIA DE CONTENIDO.",
    "EL CUADRO AZUL DE REDUCCIÓN EN LOS COSTOS DE TITULACIÓN DEBE MANTENERSE SIEMPRE.",
    "NO ELIMINAR NUNCA EL CUADRO AZUL DE REDUCCIÓN EN LOS COSTOS DE TITULACIÓN.",
    "NO CAMBIAR EL COLOR AZUL DEL CUADRO DE REDUCCIÓN.",
    "NO CAMBIAR LA FORMA, POSICIÓN, PROPORCIÓN, BORDE, ICONO NI HEADER DEL CUADRO DE REDUCCIÓN.",
    "NO RELLENAR EL CUADRO DE REDUCCIÓN CON INFORMACIÓN DE OTROS CAMPOS.",
    "NO INVENTAR PORCENTAJES, DESCUENTOS, COSTOS NI BENEFICIOS DE TITULACIÓN.",
    "SI EL PPTX NO CONTIENE INFORMACIÓN DE REDUCCIÓN, CONSERVAR EL CUADRO VISUAL SIN INVENTAR CONTENIDO.",
    "SI EL PPTX CONTIENE INFORMACIÓN DE REDUCCIÓN, UTILIZAR ÚNICAMENTE ESA INFORMACIÓN.",
    "NO MOSTRAR POR DEFINIR, PENDIENTE, NO DISPONIBLE, NO ESPECIFICADO, POR CONFIRMAR NI A DEFINIR.",
    "LAS TILDES FALTANTES EN MAYÚSCULAS SIEMPRE DEBEN CORREGIRSE.",
    "LAS CORRECCIONES QUE CAMBIEN PALABRAS DEBEN SER APROBADAS.",
    "SI EXISTE COORDINADORA SIN TELÉFONO, SOLICITAR EL TELÉFONO ANTES DE GENERAR.",
    "EL FORMATO FINAL DEBE SER OBLIGATORIAMENTE 3:4."
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
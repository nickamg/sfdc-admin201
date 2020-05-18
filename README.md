# 🚀 Tabla de contenidos
1. [🧭 Planteamiento](#🧭-Planteamiento)
    - [Fecha examen](#Fecha-examen)
    - [Estructura del examen](#Estructura-del-examen)
    - [Conceptos clave del programa](#Conceptos-clave-del-programa)
2. [🏠 Salesforce Data Model](#🏠-Salesforce-Data-Model)
    - [Standard Fields [Campos Estándar]](#Standard-Fields-Campos-Estándar)
    - [Cambiar Standard Field Labels [Etiquetas de Campos Estándar]](#Cambiar-Standard-Field-Labels-Etiquetas-de-Campos-Estándar)
    - [Añadir Help Text [Texto de Ayuda] a un Standard Field](#Añadir-Help-Text-Texto-de-Ayuda-a-un-Standard-Field)
    - [Editar valores en Standard Picklist Fields [Campos Estándar de Menús Desplegables]](#Editar-valores-en-Standard-Picklist-Fields-Campos-Estándar-de-Menús-Desplegables)
    - [Custom Fields [Campos personalizados]](#Custom-Fields-Campos-personalizados)
    - [Crear un nuevo Custom Field](#Crear-un-nuevo-Custom-Field)
    - [Picklists [Menús desplegables]](#Picklists-Menús-desplegables)
    - [Dependent Picklists [Menús desplegables con dependencias]](#Dependent-Picklists-Menús-desplegables-con-dependencias)
    - [Lookups [Relaciones]](#Lookups-Relaciones)
    - [Lookup Filters [Filtrado de relaciones]](#Lookup-Filters-Filtrado-de-relaciones)
    - [Dependent Lookups [Lookups dependientes]](#Dependent-Lookups-Lookups-dependientes)
    - [Custom Formula Fields [Campos fórmula personalizados]](#Custom-Formula-Fields-Campos-fórmula-personalizados)
    - [Definir una Formula](#Definir-una-Formula)
    - [Cross-Object Formulas [Fórmulas entre varios objetos]](#Cross-Object-Formulas-Fórmulas-entre-varios-objetos)
    - [Page Layout [Diseño de página]](#Page-Layout-Diseño-de-página)
    - [Page Layout Editor [Editor de diseño de página]](#Page-Layout-Editor-Editor-de-diseño-de-página)
    - [Asignar un Page Layout [Diseño de página] a un Profile [Perfil]](#Asignar-un-Page-Layout-Diseño-de-página-a-un-Profile-Perfil])
    - [Record Type [Tipo de registro]](#Record-Type-Tipo-de-registro)
    - [Crear un Record Type [Tipo de registro]](#Crear-un-Record-Type-Tipo-de-registro)
    - [Record Types [Tipos de registro] con Bussiness Processes [Procesos de negocio]](#Record-Types-Tipos-de-registro-con-Bussiness-Processes-Procesos-de-negocio)
    - [Crear un Bussiness Process [Proceso de negocio]](#Crear-un-Bussiness-Process-Proceso-de-negocio)
    - [Usar History Tracking [Seguimiento histórico] para mantener Data Quality [Calidad del dato]](#Usar-History-Tracking-Seguimiento-histórico-para-mantener-Data-Quality-Calidad-del-dato)
    - [Usar Data Validation [Validación de datos] para mantener Data Quality [Calidad del dato]](#Usar-Data-Validation-Validación-de-datos-para-mantener-Data-Quality-Calidad-del-dato)
    - [Data Validation [Validación de Datos]: Required Fields [Campos Requeridos] y Unique Fields [Campos Únicos]](#Data-Validation-Validación-de-Datos-Required-Fields-Campos-Requeridos-y-Unique-Fields-Campos-Únicos)
    - [Custom Data Validation [Validación de datos personalizada]: Validation Rules [Reglas de validación]](#Custom-Data-Validation-Validación-de-datos-personalizada-Validation-Rules-Reglas-de-validación)
    - [Metodología de diseño de Validation Rules [Reglas de validación]](#Metodología-de-diseño-de-Validation-Rules-Reglas-de-validación)
    - [Relaciones Master-Detail [Maestro-Esclavo]](#Relaciones-Master-Detail-Maestro-Esclavo)
    - [Lookup Relationship [Relación Lookup] y Master Detail relationship [Relación maestro esclavo]](#Lookup-Relationship-Relación-Lookup-y-Master-Detail-relationship-Relación-maestro-esclavo)
    - [Many-to-Many Relationship [Relación Muchos-a-Muchos]](#Many-to-Many-Relationship-Relación-Muchos-a-Muchos)
    - [Repaso del Modelo de Datos](#Repaso-del-Modelo-de-Datos)
3. [🚨 Modelo de Seguridad de Salesforce](#🚨-Modelo-de-Seguridad-de-Salesforce)
    - [Security Levels [Niveles de Seguridad]](#Security-Levels-Niveles-de-Seguridad)
    - [Users [Usuarios]](#Users-Usuarios)
    - [Crear nuevos Users [Usuarios]](#Crear-nuevos-Users-Usuarios)
    - [Desactivar un User [Usuario]](#Desactivar-un-User-Usuario)
    - [Ver el User's Login History [Histórico de Login de un Usuario]](#Ver-el-Users-Login-History-Histórico-de-Login-de-un-Usuario)
    - [Lidiar con un Invalid Password [Contraseña incorrecta]](#Lidiar-con-un-Invalid-Password-Contraseña-incorrecta)
    - [Confirmar Security Setting [Configuraciones de Seguridad]](#Confirmar-Security-Setting-Configuraciones-de-Seguridad)
    - [Profiles [Perfiles]](#Profiles-Perfiles)
    - [Cómo cambia la experiencia de un usuario con un Profile [Perfil]](#Cómo-cambia-la-experiencia-de-un-usuario-con-un-Profile-Perfil)
    - [Standard Profiles [Perfiles Estándar]](#Standard-Profiles-Perfiles-Estándar)
    - [Standard Chatter Profiles [Perfiles Estándar de Chatter]](#Standard-Chatter-Profiles-Perfiles-Estándar-de-Chatter)

# 🧭 Planteamiento
## Fecha examen 
10 de Junio de 2020

## Estructura del examen
- 60 preguntas
- 90 minutos
- 65% correctas para aprobar
- Las preguntas se dividen en los siguientes apartados:
    Tema | Porcentaje
    --- | ---:
    Organization Setup | 1%
    **User Setup** | 9%
    Global User Interface | 1%
    **Security and Access** | 15%
    **Standard and Custom Objects** | 18%
    **Sales Cloud Applications** | 9%
    Service Cloud Applications | 6%
    Activity Management | 3%
    Chatter | 1%
    **Data Management** | 11%
    Content and Folder Management | 2%
    **Analytics - Reports and Dashboards** | 13%
    Workflow Automation | 7%
    Desktop and Mobile Administration | 2%
    AppExchange | 2%

## Conceptos clave del programa
- **Application** [Aplicaciones]
    - **Standard Apps:** Sales, Call Center, Marketing, Salesforce Chatter, Community Content, Site.com, App Launcher
- **Tabs** [Pestañas]: pestañas dentro de una aplicación o app
- **Objects** [Objetos]: similares a una tabla en una base de datos relacional: rows = records | columns = fields
- **Standard Objects** [Objetos Estándar]:
    - **Cuenta** [Account]: Principalmente empresas clientes de la nuestra. Cada account guarda información como el nombre, la dirección y el teléfono
    - **Contact** [Contacto]: Individuos asociados a las cuentas. Por ejemplo Pedro, Teresa y María (contacts), que trabajan para Telefónica (account)
    - **Case** [Caso]: Representa el problema que tiene un cliente para que atención al cliente lo resuelva
    - **Solution** [Solución]: Se trata de una descripción de cómo resolver un problema. Sirve para que cuando un agente de atención al cliente está resolviendo un case, tenga una referencia de cómo resolver el problema
    - **Campaign** [Campaña]: Representa una campaña, y sirve para visualizar y valorar su evolución
    - **Lead** [Cliente potencial]: Representa un posible cliente, al que se puede atacar con publicidad y llamadas para que se convierta en un contact


# 🏠 Salesforce Data Model
## Standard Fields [Campos Estándar]
- Todos los objetos tienen standard fields.
- No se pueden borrar, pero puedes ocultarlos mediante *field-level security*, o eliminarlos de las *page layouts* si no son necesarios.
- Como son predefinidos, sólo puedes:
    - Cambiar su campo *label*
    - Añadir *help text*
    - Añadir y editar valores en *picklists*

```
Setup | Customize | Name of Object | Fields
```

## Cambiar Standard Field Labels [Etiquetas de Campos Estándar]
Se cambian para que concuerden más con los requerimientos de negocio de tu compañía. Por ejemplo en lugar de *Accounts* lo puedes llamar *Farmacias*, si tu negocio se encarga de suministrar siempre a farmacias. De este modo queda más claro el propósito del campo.

```
Setup | Customize | Tab Names and Labels | Rename Tabs and Labels
```

## Añadir Help Text [Texto de Ayuda] a un Standard Field
La *Field-level help* [ayuda a nivel de campo] te permite mostrar información acerca del propósito y la función de un campo para tus usuarios. El texto se podrá ver en todas las páginas que aparezca el campo.

```
Setup | Customize | Name of object | Fields | Edit
```

## Editar valores en Standard Picklist Fields [Campos Estándar de Menús Desplegables]
Los *Standard picklist fields* [campos estándar de menús desplegables] contienen valores predefinidos, que puedes eliminar, añadir o reordenar.

```
Setup | Customize | Name of Object | Fields | Name of Field
```

## Custom Fields [Campos personalizados]
Los *Custom Fields* son nuevos campos que creas en cualquier *Standard Object* o *Custom Object* para guardar cualquier información adicional que necesites.

Como no son *Standard Fields* los puedes:
- Personalizar más
- Eliminar

```
Setup | Customize | Name of object | Fields | New
```

### Pérdida de datos al editar o eliminar un Custom Field
La mayor parte de las veces, cambiar el *data type* [tipo de dato] de un *custom field* provocará que los datos que contiene se pierdan. Si los datos se pierden, cualqier *list view* [lista] basada en el *custom field* se eliminará, y las *assignment rules* [reglas de asignación] y *escalation rules* [reglas de escalado] podrán verse afectadas. **Por esta razón, deberías modificar únicamente campos sin datos, o considerar utilizar nuevos campos.**

Eliminar un campo también resultará en la pérdida de datos. Como precaución, **Salesforce guarda campos eliminados y sus datos por un máximo de 45 días**, durante los cuales puedes deshacer la eliminación o eliminarlos permanentemente.

## Crear un nuevo Custom Field
- Hay cuatro pasos para crear nuevos campos en un objeto. La información necesaria para cada paso es diferente según el tipo de campo que estemos creando. Campos de tipo *Formula, Roll-Up-Summary y Lookup* tienen pasos adicionales.
- Los pasos son los siguientes:
    1. Seleccionar el *Data Type* [Tipo de Dato]
        - Currency [Moneda]
        - Date [Fecha]
        - Checkbox
        - Picklist [Menú desplegable]
        - Text, etc [Texto, etc]
    2. Introducir los detalles
        - Label [Etiqueta]
        - Length [Longitud]
        - Picklist values [Valores del desplegable]
        - Description [Descripción]
        - Help text [Texto de ayuda]
    3. Configurar la *field-level security* [seguridad a nivel de campo]:
        - Visibilidad por *profile* [perfil]
        - Editabilidad por *profile* [perfil]
    4. Añadir a *page layouts* [diseños de página]:
        - Configurar en qué *page layouts* [diseños de página] aparece el campo

```
Setup | Customize | Name of object | Fields | New
```

## Picklists [Menús desplegables]
Son campos que permiten a los usuarios seleccionar tanto uno *(Picklist)* como varios valores *(Multi-Select Picklist)* de una lista. Puedes utilizarlos para:
- Facilitar la introducción de datos
- Mantener la calidad del dato permitiendo introducir únicamente valores concretos
- Facilitar la búsqueda, el filtrado y el reporte

## Dependent Picklists [Menús desplegables con dependencias]
Puedes enlazar dos picklists para crear una *controlling-dependent relationship* [relación controlador-dependencia]. Los usuarios seleccionan un valor en una *controlling picklist* [menú desplegable controlador], que filtra los valores disponibles en una segunda *dependent picklist* [menú desplegable dependiente].

### Cosas a tener en cuenta
- Las picklists *dependent* [dependientes] te dan la capacidad de crear dependencias a varios niveles.
- Los *field types* [tipos de campo] que soportan son los siguientes:
    Field Type | Controlling | Dependent
    --- | :---: | :---:
    Standard Picklist | Sí | No
    Custom Picklist | Sí | Sí
    Custom Multi-Select Picklist | No | Sí
    Standard Checkbox | Sí | No
    Custom Checkbox | Sí | No

## Lookups [Relaciones]
Las *lookups* [relaciones] son campos que permiten a los usuarios seleccionar un registro de otro objeto, incluyendo el *User object* [objeto Usuario], cuando insertan nuevos datos. De este modo, pueden enlazar dos registros, creando una *parent-child relationship* [relación padre-hijo].

## Lookup Filters [Filtrado de relaciones]
Utiliza un *lookup filter* [filtrado de relaciones] para limitar los registros que se pueden relacionar.

Un *Lookup Filter* puede referenciar:
- Otros campos en el mismo registro (*source* [fuente])
- Campos en los registros del *lookup object* [objeto relacionado] (*target* [objetivo])
- Campos en el *user record* [registro del usuario], *profile* [perfil], y *role* [rol]
- Campos en registros directamente relacionados al *target object* [objeto objetivo]

## Dependent Lookups [Lookups dependientes]
Utiliza un *lookup filter* [filtro de relación] que referencia otro campo en el mismo *object* [objeto] para crear una *dependent lookup* [relación de dependencia].

## Custom Formula Fields [Campos fórmula personalizados]
Los *custom formula fields* [campos fórmula personalizados] te permiten definir cálculos que referencian otros campos para mostrar  nuevos datos de tipo *numeric* [numérico], *text* [texto], *checkbox*, *currency* [moneda] o *date* [fecha] específicos a tus requerimientos de negocio.

- Son **únicamente de lectura** y no se muestran a la hora de crear un nuevo registro (ya que son calculados y el usuario no puede introducirles un valor directamente)
- Pueden referenciar campos en el mismo objeto, o en un *parent object* [objeto padre] o *lookup object* [objeto relacionado]
- No puede referenciar *currency codes* [códigos de moneda], *description* [descripciones] o *custom long text area fields* [campos de texto largo personalizados], o *multi-select picklists* [menús desplegables de selección múltiple].
- No son buscables, ni están disponibles para conversión de *leads* [clientes potenciales] o *data exports* [exportación de datos].

## Definir una Formula
Puedes definir una *formula* a través de de un paso adicional en el *custom field wizard* [la guía de creación de un campo personalizado].

## Cross-Object Formulas [Fórmulas entre varios objetos]
Una *cross-object formula* [fórmula entre varios objetos] referencia campos de *parent objects* [objetos padre]. Utiliza la *Insert Field Browser* [insertar buscador de campos] en la *Advanced Formula Tab* [pestaña de fórmula avanzada] para acceder a campos de hasta 10 padres relacionados.

## Page Layout [Diseño de página]
Una *page layout* [diseño de página] controla los *fields* [campos], *sections* [secciones], *related lists* [listas relacionadas] y *buttons* [botones] que aparecen cuando los usuarios ven o editan un registro. Puedes modificar la *default page layout* [diseño de página por defecto] de un objeto o crear nuevas *page layouts*.

```
Setup | Customize | Name of Object | Page Layouts
```

## Page Layout Editor [Editor de diseño de página]
Modifica o crea *page layouts* [diseños de página] utilizando el editor *drag-and-drop* [arrastra-y-suelta (editor mediante clicks y no código)].

```
Setup | Customize | Name of Object | Page Layouts
```

## Asignar un Page Layout [Diseño de página] a un Profile [Perfil]
Para asegurar que los usuarios ven la *page layout* [diseño de página] correcta, asigna *page layouts* a *user profiles* [perfiles de usuario].

## Record Type [Tipo de registro]
Los *record types* [tipos de registro] te permiten ofrecer a los usuarios diferentes *page layouts* [diseños de página] y *pìcklist values* [valores en menús desplegables] para distintos tipos de escenarios comerciales basándose en sus *profiles* [perfiles]. 

Por ejemplo, si tenemos un negocio que vende a fruterías y carnicerías, donde cada frutería y carnicería es una Account, necesitamos campos específicos para cada tipo de Account, dependiendo de si es frutería o carnicería. Para ello crearíamos dos *record types* [tipos de registro] en el objeto Account, uno para fruterías y otro para carnicerías.

Cada objeto tiene un *default master record type* [tipo de registro maestro por defecto], pero siempre puedes crear nuevos.

## Crear un Record Type [Tipo de registro]
Puedes crear un nuevo *record type* [tipo de registro] en unos pocos pasos. Empieza por crear la *page layout* [diseño de página] que los usuarios verán cuando trabajen con el *record type* que vas a crear, y comprueba que las *picklists* [menús desplegables] tienen todos los valores requeridos.

El proceso es el siguiente:
1. Preparación:
    - Crear la *page layout* [diseño de página]
    - Asegurar que los valores de las *picklists* [menús desplegables] están rellenos
2. Crear el *record type* [tipo de registro]:
    - Paso 1:
        - *Name* [Nombre]
        - *Description* [Descripción]
        - *Assign to profiles* [Asignación a perfiles]
    - Paso 2:
        - Selecciona el *page layout* [diseño de página] para cada *profile* [perfil]
3. Editar las *picklists* [menús desplegables]:
    - Selecciona los valores de las *picklists* [menús desplegables]

```
Setup | Customize | Name of Object | Record Types
```

## Record Types [Tipos de registro] con Bussiness Processes [Procesos de negocio]
*Opportunities* [oportunidades], *cases* [casos], *solutions* [soluciones], y *leads* [clientes potenciales], tienen cada uno un *special picklist field* [campo menú desplegable especial], llamado *bussiness process* [proceso de negocio] que te permite definir etapas para cada uno de estos objetos. 

De este modo puedes definir que un *case* [caso] tenga el siguiente *bussiness process* [proceso de negocio]:
> Nuevo &rarr; Revisado &rarr; Cliente contactado &rarr; Esperando respuesta &rarr; Caso cerrado

Puedes crear nuevas versiones para utilizar en los distintos *record types* [tipos de registro] para que representen mejor distintos escenarios de negocio.

> ⚠ Debes crear al menos un *bussiness process* [proceso de negocio] antes de que puedas crar un *record type* [tipo de registro] para los objetos anteriormente mencionados.

## Crear un Bussiness Process [Proceso de negocio]
Debes definir tus *bussiness processes* [procesos de negocio] requeridos antes de crear *record types* [tipos de registro] para *opportunities* [oportunidades], *cases* [casos], *solutions* [soluciones] o *leads* [clientes potenciales]. Es entonces cuando puedes seleccionar el *bussiness process* [proceso de negocio] creado a la hora de crear el *record type* [tipo de registro].

Los pasos son los siguientes:
1. Actualizar la *master picklist* [el menú desplegable maestro]
    - Asegúrate de que tiene todos los valores requeridos
2. Crear el *bussiness process* [proceso de negocio]:
    - *Name* [Nombre]
    - *Description* [Descripción]
    - Selecciona valores de la *master picklist* [menú desplegable maestro]
3. Crea el *record type* [tipo de registro]
    - Selecciona el *bussiness process* [proceso de negocio] que has creado

```
Setup | Customize | Name of Object | Name of Process
```

## Usar History Tracking [Seguimiento histórico] para mantener Data Quality [Calidad del dato]
Se puede activar *history tracking* [seguimiento histórico] en un objeto para seguir los cambios de hasta 20 *standard fields* [campos estándar] o *custom fields* [campos personalizados]. Los cambios se pueden ver en la *history related list* [lista relacionada del histórico] o a través de *history reports* [reportes del histórico].

Por cada campo, el *tracking* [seguimiento] registra:
- Fecha y hora del cambio
- El *user* [usuario] que ha realizado el cambio
- El valor antiguo y el nuevo (aunque no lo registra en *multi-select picklists* [menús desplegables multi selección] ni en *large text fields* [campos de texto largos])

## Usar Data Validation [Validación de datos] para mantener Data Quality [Calidad del dato]
La *data validation* [validación de datos] te permite asegurar la integridad de los datos **antes de que se guarden**, impidiendo a los *users* [usuarios] que introduzcan valores no válidos.

Hay dos tipos:
- *Standard data validation* [validación de datos estándar]: consiste en configurar propiedades simples en el campo para asegurar que se introducen datos válidos.
    - *Field data type* [Tipo de dato del campo]: especificar de qué tipo es el campo (texto, numérico, etc.)
    - *Required field* [Campo requerido]: especificar si es requerido
    - *Unique field* [Campo único]: especifica si el valor del campo ha de ser único
- *Custom validation rules* [validación de datos personalizada]: te permite configurar condiciones más complejas, que involucren uno o más campos.

> ⚠ Las *custom validation rules* [reglas de validación personalizadas] sólo se ejecutna si no hay errores en las *standard validations* [validaciones estándar]

## Data Validation [Validación de Datos]: Required Fields [Campos Requeridos] y Unique Fields [Campos Únicos]
Ciertos *custom fields* [campos personalizados] pueden ser marcados como *required* [requeridos] y/o *unique* [únicos] para forzar a los usuarios a introducir siempre un valor, o evitar que existan registros con valores duplicados.

- *Required* [Requeridos]:
    - Es obligatorio que estén rellenos a la hora de guardar
    - **Se añaden automáticamente a todas las *page layouts* [diseños de página]**
    - No se pueden ocultar
    - Accesible a todos los *profiles* [perfiles]
    - No se puede marcar como *required* [requerido] un campo *picklist* [menú desplegable] ni *long text area* [campo de texto largo]
- *Unique* [Único]:
    - No permite guardar valores duplicados
    - Los duplicados que existan causan error
    - Sólo se puede aplicar a campos con los siguientes *data type* [tipos de dato]:
        - *Email*
        - *Number* [Numérico]
        - *Text* [Texto]

## Custom Data Validation [Validación de datos personalizada]: Validation Rules [Reglas de validación]
Una *validation rule* [regla de validación] te permite especificar tus propios criterios de validación para prevenir que los *users* [usuarios] introduzcan datos no válidos en uno o más campos.

Por ejemplo, se establece que un campo descuento en el objeto *Opportunity* [Oportunidad] no debería exceder el 20%. Si un usuario intenta introducir un valor mayor, se le impedirá.

```
Setup | Customization | Name of Object | Validation Rules
```

## Metodología de diseño de Validation Rules [Reglas de validación]
Sigue un proceso consistente para asegurar que tienes reglas bien diseñadas:
1. Indica tus requerimientos de negocio de una forma descriptiva &rarr; El usuario ha de introducir una *Fecha de Finalización del Período de Garantía* cuando el campo *Tiene Garantía* está seleccionado
2. Descompón la descripción en una o más frases simples que describan los errores de validación &rarr; El usuario no debe ser capaz de guardar la *opportunity* [oportunidad] si:
    - El campo *Tiene garantía* está seleccionado
    - El campo *Fecha de Finalización del Período de Garantía* está en blanco
3. Expresa la condición del error como un booleano utilizando el lenguaje de fórmula:
    ```
    Tiene_Garantia__c = True && ISBLANK(Fecha_Finalizacion_Periodo_Garantia__c)
    ```
4. Genera un mensaje de error que responda a esta *error condition* [condición de error] &rarr; "La Fecha de Finalización del Período de Garantía ha de introducirse cuando una cuenta tiene una garantía."

## Relaciones Master Detail [Maestro Esclavo]
- Este tipo de relaciones relacionan estrechamente objetos, de tal modo que el *master record* [registro maestro] controla ciertos comportamientos de *detail record* [registro esclavo]. Cuando un *master record* [registro maestro] es eliminado, el *detail record* [registro esclavo] relacionado se elimina también.
- El campo *Owner* [Propietario] en el *detail record* [registro esclavo] no está disponible y se asocia automáticamente al *owner* [propietario] del *master record* [registro maestro]. Los *custom objects* [objetos personalizados] que sean *detail* [esclavos] en una relación *master-detail* [maestro-esclavo] no pueden tener *sharing rules* [reglas de compartir], *manual sharing* [compartir de forma manual], o *queues* [colas de espera], ya que estas requieren el campo *Owner* [Propietario].
- Las configuraciones de seguridad del *master record* [registro maestro] controlan las del *detail record* [registro esclavo].
- El campo *master-detail relationsihip* [relación maestro-esclavo] (el cual es el que une ambos objetos) se requiere en la *page layout* [diseño de página] del *detail record* [registro esclavo].
- El *master object* [objeto maestro] puede ser un *standard object* [objeto estándar], como una *Account* [Cuenta] u *Opportunity* [Oportunidad], o un *custom object* [objeto personalizado].

## Lookup Relationship [Relación Lookup] y Master Detail relationship [Relación Maestro Esclavo]
Attributes [Atributos] | Lookup | Master Detail
--- | :---: | :---:
¿Se requiere el campo *Lookup* [Relación] en el registro hijo? | No | Sí
¿Puede cambiarse el campo *Lookup* [Relación] del hijo? | Sí | No
¿Qué pasa cuando el *parent record* [registro padre] se borra? | Los *child records* [registros hijo] no se borran | Los *child records* [registros hijo] se borran
¿Puede el *parent record* [registro padre] tener *roll-up summary fields* [campos de sumario]? | No | Sí (hasta 10)
¿Cuáles son las implicaciones en materia de seguridad? | Controlado por OWD | Reglas de compartir heredadas del padre
¿Cuáles son las implicaciones a la hora del reporting? | Sólo están disponibles los campos del hijo | Todos los campos del padre y el hijo están disponibles.

## Many-to-Many Relationship [Relación Muchos-a-Muchos]
- Puedes utilizar una relación *master-detail* [maestro-esclavo] para modelar una relación *many-to-many* [muchos-a-muchos] entre dos *standard objects* [objetos estándar], dos *custom objects* [objetos personalizados], o un *custom object* [objeto personalizado] y un *standard object* [objeto estándar].
- Una relación *many-to-many* [muchos-a-muchos] permite relacionar un registro de un objeto a múltiples registro de otro objeto y al revés.
- Por ejemplo, puedes tener un *custom object* [objeto personalizado] llamado "Bug", que se relaciona con el objeto estándar *case* [caso], de tal forma que el objeto "Bug" puede relacionarse a múltiples casos, y un caso puede relacionarse con múltiples bugs.
- Las relaciones *many-to-many* requieren un objeto intermedio. En este caso podría representarse del siguiente modo:
    > Case &larr;&rarr; Objeto Intermedio &larr;&rarr; Bug

## Repaso del Modelo de Datos
- *Standard Fields* [Campos Estándar]
- *Custom Fields* [Campos Personalizados]
- *Picklists* [Menús desplegables]
- Enlazar campos con *Dependent Picklists* [Menús Desplegables Dependientes]
- Enlazar *Objects* [Objetos] mediante *Lookups* [Relaciones]
- Formulas
- Personalizar la representación de los datos:
    - *Page Layout* [Diseño de página]
    - *Record Type* [Tipo de registro]
    - *Bussiness Process* [Proceso de negocio]
- *Master-Detail Relationship* [Relación Maestro-Esclavo]
- *Many-to-Many Relationship* [Relación Muchos-a-Muchos]

# 🚨 Modelo de Seguridad de Salesforce

## Security Levels [Niveles de Seguridad]
*Organization* [Organización] &rarr; *Object* [Objeto] &rarr; *Record* [Registro] &rarr; *Field* [Campo]

```
+- Organization ----------------+
|                               |
|  +- Object ----------------+  |
|  |                         |  |
|  |  +- Record ----------+  |  |
|  |  |                   |  |  |
|  |  |  +- Field -----+  |  |  |
|  |  |  |             |  |  |  |
|  |  |  +-------------+  |  |  |
|  |  +-------------------+  |  |
|  +-------------------------+  |
+-------------------------------+
```

## Users [Usuarios]
Un usuario es alguien con *login access* [acceso mediante login] a la *Salesforce organization* [la organización de Salesforce], que tiene una licencia y un *user record* [registro de usuario] que contiene información acerca de la seguridad, *locale* [localización (idioma, moneda, hora, etc.)] e información personal.
Personal | *Security & Access* [Seguridad y acceso] | *Locale* [Localización]
:--- | :--- | :---
*Name* [Nombre] | *Username* [Nombre de usuario] | *Time Zone* [Zona horaria]
Alias | *License(s)* [Licencia(s)] | *Locale* [Localización]
Email | *Profile* [Perfil] | *Language* [Idioma]
*Phone/Address* [Teléfono/Dirección] | *Role* [Rol] | *Currency* [Moneda]
*Title* [Título] | *Login History* [Histórico de login]

```
Setup | Manage Users | Users
```

## Crear nuevos Users [Usuarios]
Puedes crear uno o varios usuarios con únicamente la información requerida. La opción *Generate new password* [Generar nueva contraseña], seleccionada por defecto, enviará un email al usuario con el *username* [nombre de usuario] y una *temporary password* [contraseña temporal].

## Desactivar un User [Usuario]
Los registros de *Users* [Usuarios] **no pueden ser eliminados**, pero pueden ser desactivados.

La desactivación:
- Mantiene la integridad del histórico (se mantiene el registro de lo que hizo ese usuario)
- Previene que el usuario acceda a nuestra organización de Salesforce
- Libera una *user license* [licencia de usuario]

## Ver el User's Login History [Histórico de Login de un Usuario]
La *Login History Related List* [lista relacionada del histórico de login] del registro de un *user* [usuario] muestra cuándo, dónde y cómo intenta loguearse un usuario. Utiliza la columna *Status* [Estado] para diagnosticar cualquier problema con el login. Si no hay ningún registro aquí que muestre el intento de loguearse de un usuario, el usuario probablemente esté utilizando un *username* [nombre de usuario] incorrecto.

```
Setup | Manage Users | Users | Name of User
Setup | Manage Users | Login history
```

## Lidiar con un Invalid Password [Contraseña incorrecta]
Es buena práctica permitir que los usuarios reinicien sus contraseñas haciendo click en el enlace *"Forgot your password?"* ["Olvidaste tu contraseña?"] en la página de login. Si continúan sin poder acceder, puedes reiniciarles la contraseña de forma manual.

```
Setup | Manage Users | Users
```

## Confirmar Security Setting [Configuraciones de Seguridad]
Un *Password Lockout* [bloqueo de contraseña] ocurre cuando tienes una *password policy* [política de contraseñas] que bloquea usuarios que exceden un cierto número de intentos de login erróneos. El período de bloqueo puede ser temporal o puede requerir un *admin reset* [reinicio manual por parte de un administrador]. Puedes desbloquear a un usuario haciendo click en **_Unlock_** en el registro del usuario.

```
Setup | Security Controls | Password Policies
```

## Profiles [Perfiles]
Un *profile* [perfil] es una coleccion de *settings* [configuraciones] y *permissions* [permisos] que determinan qué pueden ver los usuarios en la interfaz, y qué pueden hacer.
Settings (lo que los usuarios ven) | Permissions (lo que los usuarios pueden hacer)
--- | ---
Apps | *Administrative* [Administrativo] (p.ej.: personalizar una app)
*Tabs* [Pestañas] | *General User* (p.ej.: realizar reportes, enviar emails)
*Record Types* [Tipos de registro] | *Standard Object* [Objeto Estándar] (p.ej.: crear *leads* [usuarios potenciales])
*Page Layouts* [Diseños de página] | *Custom Object* [Objeto Personalizado] (p.ej.: editar campos)
*Fields* [Campos] | 

## Cómo cambia la experiencia de un usuario con un Profile [Perfil]
- Qué *tabs* [pestañas] son visibles
- Qué Apps son visibles
- Qué pueden hacer con registros de un objeto concreto
- Qué campos son visibles
- Qué campos son editables
- El diseño de la página

## Standard Profiles [Perfiles Estándar]
Los *standard profiles* [perfiles estándar] no pueden ser eliminados y sus permisos no pueden ser editados.

*Standard Profile* [Pefil Estándar] | *Permissions* [Permisos]
--- | ---
*System Administrator* [Administrador de sistema] | Ver y modificar todos los datos, personalizar app
*Standard User* [Usuario Estándar] | Ver, editar y eliminar los registros que pueden acceder
*Solution Manager* [Manager de Soluciones] | *Standard User* + puede gestionar Soluciones publicadas
*Marketing User* [Usuario de Marketing] | *Standard User* + importar *Leads* [clientes potenciales]
*Contract Manager* [Manager de contratos] | *Standard User* + gestionar Contracts
*Read Only* [Sólo lectura] | Únicamente puede ver registros que pueden acceder

## Standard Chatter Profiles [Perfiles Estándar de Chatter]
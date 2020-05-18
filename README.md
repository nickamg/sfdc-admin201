# 🚀 Tabla de contenidos
1. [🧭 Planteamiento](#🧭-Planteamiento)
    - [Fecha examen](#Fecha-examen)
    - [Estructura del examen](#Estructura-del-examen)
    - [Conceptos clave del programa](#Conceptos-clave-del-programa)
2. [🏠 Salesforce Data Model](#🏠-Salesforce-Data-Model)
    - [Standard Fields [Campos Estándar]](#Standard-Fields-Campos-Estándar)
    - [Cambiar Standard Field Labels [Etiquetas de Campos Estándar]](#Cambiar-Standard-Field-Labels-[Etiquetas-de-Campos-Estándar])
    - [Añadir Help Text [Texto de Ayuda] a un Standard Field](#Añadir-Help-Text-[Texto-de-Ayuda]-a-un-Standard-Field)
    - [Editar valores en Standard Piclist Fields [Campos Estándar de Menús Desplegables]](#Editar-valores-en-Standard-Piclist-Fields-[Campos-Estándar-de-Menús-Desplegables])
    - [Custom Fields [Campos personalizados]](#Custom-Fields-[Campos-personalizados])
    - [Crear un nuevo Custom Field](#Crear-un-nuevo-Custom-Field)
    - [Picklists [Menús desplegables]](#Picklists-[Menús-desplegables])
    - [Dependent Picklists [Menús desplegables con dependencias]](#Dependent-Picklists-[Menús-desplegables-con-dependencias])
    - [Lookups [Relaciones]](#Lookups-[Relaciones])
    - [Lookup Filters [Filtrado de relaciones]](#Lookup-Filters-[Filtrado-de-relaciones])
    - [Dependent Lookups [Lookups dependientes]](#Dependent-Lookups-[Lookups-dependientes])

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

## Editar valores en Standard Piclist Fields [Campos Estándar de Menús Desplegables]
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
    - Seleccionar el *Data Type* [Tipo de Dato]
        - Currency [Moneda]
        - Date [Fecha]
        - Checkbox
        - Picklist [Menú desplegable]
        - Text, etc [Texto, etc]
    - Introducir los detalles
        - Label [Etiqueta]
        - Length [Longitud]
        - Picklist values [Valores del desplegable]
        - Description [Descripción]
        - Help text [Texto de ayuda]

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
Utiliza un *lookup filter* [filtro de relación] que referencia otro campo en el mismo *object* [objeto] para crear una *dependent lookup* [relación de dependencia]. Por ejemplo, añade un *lookup filter*
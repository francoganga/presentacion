---
title: 
- Registro Unificado de Actividades
author:
- Franco Ganga
institute:
- Universidad Nacional Arturo Jauretche - Instituto de Ingeniería y Agronomía
theme:
- metropolis
header-includes:
- \usepackage{xcolor}
- \usepackage{listings}
---



# Problema

La Universidad no posee un sistema que administre la información sobre las actividades
realizadas por cada persona: actualmente, estos datos son almacenados en planillas excel o
documentos escritos.
El propósito de este proyecto es ofrecer una solución a este problema.


#

\begin{columns}
    \begin{column}{.5\textwidth}
    \centering
    \fontsize{20}{10}\selectfont
        \textbf{
                Objetivos
        }
    \end{column}
    \begin{column}{.5\textwidth}
    \includegraphics[width=\textwidth]{/home/unaj/objetivos.png}
    \end{column}
\end{columns}

# Objetivos


\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \large{\textbf{Objetivos por alcanzar}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Plataforma web de administración.
                \item<2-> Integración con datos de sistemas externos.
                \item<3-> Servicio API REST.
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                \only<1>{\includegraphics[width=0.8\textwidth]{/home/unaj/web_admin.png}}
                \only<2>{\includegraphics[width=0.8\textwidth]{/home/unaj/integracion.png}}
                \only<3>{\includegraphics[width=0.8\textwidth]{/home/unaj/api.png}}
        \end{itemize}
    \end{column}
\end{columns}

# Componentes utilizados


\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \begin{itemize}
            \Large
            \item<1-> Symfony
            \item<2-> Doctrine
            \item<3-> Sonata
            \item<4-> Api-Platform
        \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                \only<1>{\includegraphics[width=0.8\textwidth]{/home/unaj/Descargas/symf_.png}}
                \only<2>{\includegraphics[width=0.8\textwidth]{/home/unaj/Descargas/symf_doctrine.png}}
                \only<3>{\includegraphics[width=0.8\textwidth]{/home/unaj/Descargas/symf_doc_sonata.png}}
                \only<4>{\includegraphics[width=0.8\textwidth]{/home/unaj/Descargas/sym_doc_son_apip.png}}
        \end{itemize}
    \end{column}
\end{columns}

# Symfony
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \large{\textbf{Características}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
        \begin{itemize}
            \item<1-> Es user-friendly.
            \item<2-> Herramientas CLI.
            \item<3-> Fácil de configurar.
            \item<4-> Comunidad grande.
            \item<5-> Buena documentación
        \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \includegraphics[width=0.5\textwidth]{/home/unaj/symfony.png}
    \end{column}
\end{columns}

#

\begin{columns}
    \begin{column}{.5\textwidth}
    \centering
    \fontsize{20}{10}\selectfont
        \textbf{
                Sonata
        }
    \end{column}
    \begin{column}{.5\textwidth}
    \includegraphics[width=\textwidth]{/home/unaj/sonata.png}
    \end{column}
\end{columns}

# Sonata


\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \large{\textbf{Qué es Sonata}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
    \begin{itemize}
        \item<1-> Interfaz de administración
        \item<2-> Integración con Doctrine
        \item<3-> Integración con FOSUser
    \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \includegraphics[width=0.5\textwidth]{/home/unaj/sonata3.png}
    \end{column}
\end{columns}




# Acciones: Lista

\includegraphics[width=\textwidth]{/home/unaj/sonata_lista.png}

# Acciones: Creación

\includegraphics[width=\textwidth]{/home/unaj/sonata_crear.png}

# Acciones: Edición

\includegraphics[width=\textwidth]{/home/unaj/sonata_editar.png}

# Doctrine

\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \large{\textbf{ORM: Doctrine}}
        {\color{custom}\par\noindent\rule{\textwidth}{0.9pt}}
    \begin{itemize}
        \item<1-> Basado en Hibernate
        \item<2-> Integración con Sonata
        \item<3-> Migraciones
    \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \includegraphics[width=0.5\textwidth]{/home/unaj/doctrine.png}
    \end{column}
\end{columns}

#
\begin{center}
    \huge\textbf{Sonata-User}
\end{center}

# Sonata User

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.7\textwidth}
        \Large{\textbf{Qué es Sonata-User}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Integra \textbf{Sonata} y \textbf{FOSUser}
                \item<2-> Menú de usuario
                \item<3-> Soporte para autenticación mediante Google
                \item<4-> Administración de usuarios y grupos
                \item<5-> Roles
            \end{itemize}
    \end{column}
    \begin{column}{.3\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/sonata3.png}}
        \end{itemize}
    \end{column}
\end{columns}

#

\begin{center}
    \huge{\textbf{Instalación y Configuración}}
\end{center}


# Instalación y configuración

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Involucra}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Doctrine
                \item<2-> FOSUser
                \item<3-> Security
                \item<4-> Routing
                \item<5-> Sonata-User
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                \only<1>{\includegraphics[width=0.8\textwidth]{/home/unaj/suser1.png}}
                \only<2>{\includegraphics[width=0.8\textwidth]{/home/unaj/suser2.png}}
                \only<3>{\includegraphics[width=0.8\textwidth]{/home/unaj/suser3.png}}
                \only<4>{\includegraphics[width=0.8\textwidth]{/home/unaj/suser4.png}}
                \only<5>{\includegraphics[width=0.8\textwidth]{/home/unaj/integracion.png}}
        \end{itemize}
    \end{column}
\end{columns}

#
\begin{center}
    \huge{\textbf{API-Platform}}
\end{center}

# API Platform

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Qué es API Platform}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> API \textit{framework}
                \item<2-> Soporta muchos estándares de desarrollo
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/api-platform.png}}
        \end{itemize}
    \end{column}
\end{columns}

#
\begin{center}
\huge{\textbf{Serialización}}
\end{center}

# Serialización
\begin{center}
\includegraphics[width=\textwidth]{/home/unaj/serializationWorkflow.png}
\end{center}

# 

\begin{center}
    \huge\textbf{Contexto de Normalización y Desnormalización}\

    Definen propiedades presentes en cada uno de los procesos
\end{center}

# Serialización

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
        \Large{\textbf{Grupos}}
        {\color{custom}\par\noindent\rule{\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Permiten agrupar propiedades en cada contexto
                \item<2-> Siguen relaciones
            \end{itemize}



#

\begin{columns}
    \begin{column}{.5\textwidth}
    \centering
    \fontsize{20}{10}\selectfont
        \textbf{
                Modelado
        }
    \end{column}
    \begin{column}{.5\textwidth}
    \includegraphics[width=\textwidth]{/home/unaj/dbicon.png}
    \end{column}
\end{columns}

# Actividad

\includegraphics[width=\textwidth, height=0.5\textwidth]{/home/unaj/actividad-modelo.png}

# Pasantia

\includegraphics[width=\textwidth, height=0.5\textwidth]{/home/unaj/miembros_pasantia.png}

# Proyecto
\begin{center}
\includegraphics[width=0.8\textwidth, height=0.4\textwidth]{/home/unaj/mpr-new.png}
\end{center}

#

\centering\Huge \textbf{Herencia de Clase}

# Herencia de Clase

\centering\huge{Cada tabla \textit{hija} almacena sus datos en una tabla propia}

# Herencia de Clase

\centering\huge{Las tablas \textit{hijas} poseen una referencia a la id del \textit{padre}}

# Herencia de Clase

\definecolor{custom}{RGB}{196,174,84}
\Large{\textbf{Configuración}}
{\color{custom}\par\noindent\rule{\textwidth}{0.9pt}}
    \begin{itemize}
    \Large
        \item<1-> Propiedad \textbf{discriminator}
        \item<2-> Establecer la Herencia de Clase
    \end{itemize}

# Herencia de Clase {.fragile .t}

```json
{"miembro_cursoExtension" = "MiembroCursoExtension",
"rector" = "Rector"}
```

. . . 

```php
class MiembroCursoExtension extends Actividad
```



#

\centerline{\Huge\textbf{Mapeo}}
\vspace{1cm}
\centerline{\Huge\textbf{Objeto-Relacional}}

# Mapeo Objeto - Relacional: Metadata (Anotaciones)

```php
<?php
/** @Entity */
class Message
{
    /** @Column(type="integer") */
    private $id;
    /** @Column(length=140) */
    private $text;
    /** @Column(type="datetime", name="posted_at") */
    private $postedAt;
}
```

# Mapeo Objeto - Relacional: Metadata (XML)
```xml
<doctrine-mapping>
  <entity name="Message">
    <field name="id" type="integer" />
    <field name="text" length="140" />
    <field name="postedAt" column="posted_at" type="datetime" />
  </entity>
</doctrine-mapping>
```

# Mapeo Objeto - Relacional: Metadata (YAML)
```yaml
Message:
  type: entity
  fields:
    id:
      type: integer
    text:
      length: 140
    postedAt:
      type: datetime
      column: posted_at
```

#
\begin{columns}
    \begin{column}{.5\textwidth}
    \centering
    \fontsize{20}{10}\selectfont
        \textbf{
                Relaciones
        }
    \end{column}
    \begin{column}{.5\textwidth}
    \includegraphics[width=\textwidth]{/home/unaj/relaciones.png}
    \end{column}
\end{columns}

# Relaciones

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Tipos de Relaciones}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \Large
                \item<1-> Unidireccionales
                \item<2-> Bidireccionales
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                \only<1>{\includegraphics[width=0.8\textwidth]{/home/unaj/unidireccional.png}}
                \only<2>{\includegraphics[width=0.8\textwidth]{/home/unaj/bidireccional2.png}}
        \end{itemize}
    \end{column}
\end{columns}

# 

\begin{center}
  \begin{itemize}
    \centering
    \setlength\itemsep{1em}
    \item[]<1-> \huge{\textbf{Lado Propietario}}
    \item[]<2-> \huge{Doctrine solo comprueba este lado por cambios en la relación}
  \end{itemize}
\end{center}


#

\begin{center}
    \huge\textbf{Clases Administradoras}\

    Definen qué hacer en cada acción
\end{center}

# Clases Administradoras
\setbeamercovered{transparent}
\definecolor{custom}{RGB}{196,174,84}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Qué es necesario}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
        \begin{itemize}
            \item<1-> Definir la Clase
            \item<2-> Establecerla como servicio
        \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \includegraphics[width=0.5\textwidth]{/home/unaj/sonata3.png}
    \end{column}
\end{columns}

#

\begin{columns}
    \begin{column}{.5\textwidth}
    \centering
    \fontsize{20}{10}\selectfont
        \textbf{
                Ejemplos
        }
    \end{column}
    \begin{column}{.5\textwidth}
    \includegraphics[width=0.7\textwidth]{/home/unaj/code.png}
    \end{column}
\end{columns}

# Iserción o Edición

```php

public function configureFormFields(
    FormMapper $formMapper
    ): void
{
    $formMapper
        ->add('persona', ModelListType::class)
        ->add('inicio', DatePickerType::class)
        ->add('fin', DatePickerType::class)
        ;
}

```

# Lista


```php
public function configureListFields(
    ListMapper $listMapper
    ): void
{
    $listMapper
        ->add('persona.nombre', null, [
            'label' => 'Nombre'
            ])
        ->add('persona.apellido', null, [
            'label' => 'Apellido'
            ])
        ->add('inicio')
        ->add('fin')
}

```

# Visualización

```php
public function configureShowFields(
    ShowMapper $showMapper
    ): void
{
    $showMapper
        ->add('persona.nombre', null, [
            'label' => 'Nombre'
            ])
        ->add('persona.apellido', null, [
            'label' => 'Apellido'
            ])
        ->add('inicio')
        ->add('fin')
        ;
}
```

# Servicio



```yaml
admin.movilidad_rtf:
    class: App\Admin\MovilidadRTFAdmin
    arguments: [~, App\Entity\MovilidadRTF, ~]
    tags:
        - { 
        name: sonata.admin,
        manager_type: orm,
        group: admin,
        label: MovilidadRTF 
        }
    public: true
```

#

\begin{center}
    \huge\textbf{Admins}\
\end{center}

# Admins Simples

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Actividades simples}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Involucran una única persona
                \item<2-> Duplicación de código
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/admin-icon.png}}
        \end{itemize}
    \end{column}
\end{columns}

# Solución {.b}

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.8\textwidth}
        \Large{\textbf{Traits}}
        {\color{custom}\par\noindent\rule{1\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Métodos redefinidos por orden de precedencia
                \item<2-> Cada admin mantiene su propia clase
                \item<3-> Más flexible
            \end{itemize}
    \end{column}
    \begin{column}{.2\textwidth}
        \vfill
        {\includegraphics[width=0.8\textwidth]{/home/unaj/trait.png}}
    \end{column}
\end{columns}


#

\begin{center}
    \huge\textbf{Admins Compuestos}\
\end{center}

# Admins Compuestos

\definecolor{custom}{RGB}{196,174,84}
\begin{columns}[T]
    \begin{column}{.6\textwidth}
        \Large{\textbf{En qué consiste}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
    \begin{itemize}
        \item<2-> Cada acción del \textit{hijo} es accedida a través del \textit{padre}
        \item<3-> Se obtienen rutas anidadas
    \end{itemize}
    \end{column}
    \begin{column}{.4\textwidth}
        \includegraphics[width=0.5\textwidth]{/home/unaj/sonata3.png}
    \end{column}
\end{columns}

# Admins Compuestos


\centerline{\huge Rutas base de }
\vspace{3mm}
\centerline{\huge Miembros de proyecto:}
\begin{center}
\textbf{\large/miembroproyecto/{id}/(show | edit)}
\textbf{\large/miembroproyecto/list}
\end{center}

# Admins Compuestos
\centerline{\huge Resultado de definir Proyecto }
\centerline{\huge como padre de miembro:}
\begin{center}
\large\textbf{/proyecto/\{id\}/miembroproyecto/\{id\}/(show | edit)}\

\textbf{/proyecto/\{id\}/miembroproyecto/list}
\end{center}

# Asignación de hijo en el servicio

```yaml
- [addChild, ['@admin.miembro_proyecto', 'proyecto']]
```

# Resultado

\includegraphics[width=\textwidth]{/home/unaj/sonata_child_list.png}

# Resultado

\includegraphics[width=\textwidth]{/home/unaj/sonata_child_list_2.png}

#

\begin{center}
    \huge{\textbf{Vista de Persona}}
\end{center}

# Vista de Persona

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Información a Exponer}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Listado de Actividades
                \item<2-> Datos de la Persona
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/web_admin.png}}
        \end{itemize}
    \end{column}
\end{columns}

# Vista de Persona

    
\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.6\textwidth}
        \Large{\textbf{Cómo de logró}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Iteración de colección de actividades
                \item<2-> Se crea un contenedor por cada actividad
                \item<3-> Se agregan botones y títulos correspondientes
            \end{itemize}
    \end{column}
    \begin{column}{.4\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.7\textwidth]{/home/unaj/dev.png}}
        \end{itemize}
    \end{column}
\end{columns}

# Vista de Persona
\begin{center}
\includegraphics[width=\textwidth]{/home/unaj/PPSDOC/image/vista_persona.png}
\end{center}

#

\begin{center}
    \huge{\textbf{Integración con Mapuche}}
\end{center}

# Integración: Mapuche

\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{En qué consiste}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Obtención de datos externos a través de HTTP
                \item<2-> Llenar entidades con datos obtenidos
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/api.png}}
        \end{itemize}
    \end{column}
\end{columns}

#

\begin{center}
    \huge{\textbf{Eventos}}
\end{center}

# Eventos

\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \Large{\textbf{Cómo funcionan}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
            \begin{itemize}
                \item<1-> Notificaciones
                \item<2-> Listeners y Subscribers
            \end{itemize}
    \end{column}
    \begin{column}{.5\textwidth}
        \begin{itemize}[<+->]
            \item[]
                {\includegraphics[width=0.8\textwidth]{/home/unaj/symfony.png}}
        \end{itemize}
    \end{column}
\end{columns}


#    
\begin{center}
    \huge\textbf{Eventos: Doctrine}\
    
    Relacionados al ciclo de vida de una entidad

\end{center}

    
#

\begin{center}
    \huge{\textbf{PostLoad}}

    Una vez que la entidad es cargada
\end{center}

# Integración




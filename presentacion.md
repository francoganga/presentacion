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
        {\color{custom}\par\noindent\rule{1.3\textwidth}{0.9pt}}
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

# Herencia de clase

\huge{Cada tabla \textit{hija} almacena sus datos en una tabla propia}

# Herencia de clase

\huge{Las tablas \textit{hijas} poseen una referencia a la id del \textit{padre}}

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
                \large
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

# Lados de la Relación {.t}
\definecolor{custom}{RGB}{196,174,84}
\Large{\textbf{Tipos de Relaciones}}
\vspace{0pt}
\color{custom}\par\noindent\rule{0.7\textwidth}{0.9pt}



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
        \large{\textbf{Qué es necesario}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
        \begin{itemize}
            \item<1-> Definir la clase
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
    \huge\textbf{Admins Compuestos}\
\end{center}

# Admins Compuestos

\definecolor{custom}{RGB}{196,174,84}
\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.6\textwidth}
        \large{\textbf{En qué consiste}}
        {\color{custom}\par\noindent\rule{1.2\textwidth}{0.9pt}}
    \begin{itemize}
        \item<1-> Cada acción del \textit{hijo} es accedida a través del \textit{padre}
        \item<2-> Se obtienen rutas anidadas
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


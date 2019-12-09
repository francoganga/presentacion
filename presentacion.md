---
title: 
- Registro Unificado de Actividades
author:
- Franco Ganga
theme:
- metropolis
header-includes:
- \usepackage{listings}
- \usepackage{xcolor}
---



# Problema

La Universidad no posee un sistema que administre la información sobre las actividades
realizadas por cada persona: actualmente, estos datos son almacenados en planillas excel o
documentos escritos.
El propósito de este proyecto es ofrecer una solución a este problema.

# Objetivos


\begin{itemize}
    \item<1-> Plataforma web de administración.
    \item<2-> Integración con datos de sistemas externos.
    \item<3-> Servicio API REST.
\end{itemize}

# Componentes utilizados


\setbeamercovered{transparent}
\begin{columns}[T]
    \begin{column}{.5\textwidth}
        \begin{itemize}
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

\input{testInput.tex}

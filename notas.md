# Curso de Git y GitHub

## Clase 30 - Gestion de Tokens para Acceso Seguro a Repositorios

GitHub Tokens permite que terceros utilicen la base de codigo de manera segura y temporal. Este permite otorgar:

- Privilegios
- Alcance de visibilidad predefinido

Para generar un token la direccion es la siguiente:

- GitHub-> Profile-> Settings-> Developer Setting

Un ejemplo de un token clasico es el siguiente:

- `ghp_KGhazuv0Q2yaUjykcWSHoMpKY7wLWNQ3XYgIJ`

Un ejemplo de un token de grado fino es el siguiente:

- `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`

|Clasico| De grado fino|
|-|-|
|Propositos generales|Permisos especificos |

Los tokens pueden ser borrados despues de su creacion pero token como tal solo es visible una vez.

## Clase 31 - Seguridad de Paquetes con DependaBot

Dependabot es un bot el cual verifica la seguridad en los paquetes instaladaos: control de versiones, vulnerabilidades, nivel de amenaza, etc...

Es posible activar el bot de la siguiente manera:

1. Navegamos a los setting del proyecto: 
    - User-> Repo-> Settings-> Advanced Security

2. Activamos las funcionalidades que queremos utilizar: Alertas, Actualziaciones de seguridad, etc... 

El bot encuentra el problema y realiza una solucion con un PR utilizando diferentes ramas para evitar conflictos.

## Clase 32 - Configuracion Repositorios Privados

La seguridad se puede basar en diferentes aspectos, estos se pueden categorizar como tips: 

1. Hacer el repositorio privado
    - Esto evita que terceros vean como esta estructurado el codigo base de la aplicación

2. .gitignore
    - Ignora elementos los cuales se pretende mantener en privado

3. Autenticacion de dos factores

4. Configura alertas de seguridad

5. Revoca claves expuestas
    - Si se sube informacion sensible, revoca claves inmediatamente y rota las credenciales

## Clase 33 - Mitigacion Brechas de Seguridad

Esta mitigacion funciona con el uso del secret scanning. Esa herramienta sirve para prevenir y/o combatir brechas de seguridad con información sensible: api keys, passwords, etc...

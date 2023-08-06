---
icon: 
  type: line-md:edit
  color: e2ac08 
---
# Elementos de seguridad
Aspectos de seguridad del sitio web y los repositorios

[[toc]]

## Protecciones de rama
Como medida de seguridad para evitar la edición no avalada del sitio web principal, se habilitaron las protecciones de rama como se puede visualizar en el siguiente PDF adjuntado. No se recomienda deshabilitar ni debilitar dichas reglas.

- [PDF con referencia de protecciones de rama](archivos/ruleset.pdf)

En dichas reglas se estableció un requisito de 10 aprobaciones para poder incorporar un Pull Request, para así evitar colusión para la modificación indebida del sitio web. Este requisito puede ser omitido por la cuenta del TCU.

## Incorporación de estudiante colaboradores

Si el [repositorio](https://github.com/tc-565/inicio) del sitio web principal es privado, para que este sea visible por los estudiantes para poder subir un issue hay dos opciones:

- (Más seguro) Que los estudiantes provean los enlaces de sus repositorios por un medio distinto a GitHub, y que no tengan acceso al código fuente del sitio [https://github.com/tc-565/inicio](https://github.com/tc-565/inicio).
- Incorporar a los estudiantes como colaboradores con bajos privilegios en el [repositorio](https://github.com/tc-565/inicio).
	1. En el repositorio del sitio web principal, vaya a `Settings`.
 	2. En la barra lateral seleccione `Collaborators`.
  	3. Seleccione `Add people`.
  	4. Digite el correo institucional del estudiante que desea incluir, ya que este debió haber creado su cuenta de GitHub con dicho correo, o asociar el correo a su cuenta existente. 

No hay ningún otro motivo para darle acceso y privilegios adicionales a un estudiante en el repositorio del sitio web principal.
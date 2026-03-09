
# Infrastructura como Codigo

A brief description of what this project does and who it's for

# Proyecto IaC - Infraestructura como Código

## Descripción

Este repositorio contiene scripts de Infraestructura como Código (IaC) desarrollados con Terraform.
El objetivo es automatizar la creación de infraestructura mediante archivos de configuración.

La infraestructura creada incluye:

* Creación de Red
* Creación de Recurso de cómputo
* ACreación de Almacenamiento

Estos recursos se crean automáticamente mediante scripts versionados en Git.

---

# Estructura del proyecto

El repositorio contiene los siguientes archivos:

compute.tf
Define el recurso de cómputo que se desplegará en la infraestructura.

network.tf
Define los recursos de red necesarios para el funcionamiento del entorno.

storage.tf
Define el recurso de almacenamiento utilizado en la infraestructura.

main.tf
Configura el proveedor de infraestructura que utilizará Terraform.

README.md
Contiene la documentación del proyecto y los pasos para ejecutar los scripts.

---

# Requisitos

Antes de ejecutar el proyecto es necesario contar con:

* Terraform instalado
* Git instalado
* Acceso a una cuenta de proveedor de nube
* Credenciales configuradas para Terraform

---

# Clonar el repositorio

```bash
git clone https://github.com/usuario/repositorio.git
```

Entrar a la carpeta del proyecto:

```bash
cd repositorio
```

---

# Inicializar Terraform

```bash
terraform init
```

Este comando descarga los plugins necesarios para el proveedor de infraestructura.

---

# Verificar el plan de infraestructura

```bash
terraform plan
```

Este comando muestra los recursos que se crearán antes de aplicarlos.

---

# Crear la infraestructura

```bash
terraform apply
```

Terraform pedirá confirmación para crear los recursos.

Escribir:

yes

Después de esto se crearán automáticamente:

* Red
* Recurso de cómputo
* Recurso de almacenamiento

---

# Eliminar la infraestructura

Si se desea eliminar los recursos creados se puede ejecutar:

```bash
terraform destroy
```

---

# Evidencia de funcionamiento

Para comprobar que la infraestructura se creó correctamente se debe:

1. Ejecutar correctamente el comando `terraform apply`
2. Verificar que los recursos aparecen creados
3. Confirmar que no hay errores en la ejecución

Las evidencias pueden presentarse mediante capturas de pantalla del proceso de creación de la infraestructura.

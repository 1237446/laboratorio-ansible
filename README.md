# laboratorio-ansible
Infraestructura para desplegar un laboratorio de Ansible de manera local usando contenedores Docker.

> [!WARNING]
> **Entorno inseguro por diseño.**
> Para simplificar la puesta a punto de una infraestructura compleja de aprendizaje, los contenedores se ejecutan con configuraciones deliberadamente inseguras:
> - Modo `privileged` activo (acceso total al kernel del host).
> - `cgroup: host` compartido entre contenedor y host.
> - Volumen `/sys/fs/cgroup` montado en modo escritura.
> - Docker-in-Docker (DinD) habilitado.
>
> **No uses este laboratorio en producción ni expongas los contenedores a internet sin un control de acceso adicional.**

# PPS-Unidad1Actividad4-MansurSY

En esta actividad vamos a trabajar sobre la prueba de aplicaciones en entornos controlados: sandboxex o cajas de arena.

Puedes ver en qué consiste y diferentes alternativas en el siguiente artículo:b https://www.hysolate.com/learn/sandboxing/what-is-app-sandboxing/

La actividad consiste en probar la aplicación de la calculadora, que has realizado en una actividad anterior, en un entorno controlado. (Si no la tienes terminada, puedes usar la que tienes adjunta en la tarea)

  Busca cuáles son las distintas alternativas que tienes para probar esta aplicación en una Sandbox.

  1. Máquinas Virtuales (VM)
  
      Descripción: Una máquina virtual es un sistema operativo completamente aislado que se ejecuta dentro de otro sistema operativo, utilizando software como VMware, VirtualBox o Hyper-V.
      Ventajas: Total aislamiento del sistema anfitrión; fácil de configurar y destruir; puedes tener una máquina específica para pruebas sin que interfiera en tu entorno de trabajo.
      Desventajas: Puede ser costoso en términos de recursos, ya que cada VM necesita suficiente memoria y potencia de CPU.
  
  2. Contenedores (Docker, Podman)
  
      Descripción: Los contenedores permiten ejecutar aplicaciones en entornos aislados pero compartiendo el mismo sistema operativo subyacente. Docker es el sistema más popular para esto.
      Ventajas: Son más ligeros que las máquinas virtuales porque no requieren un sistema operativo completo, solo las dependencias necesarias. Son muy rápidos para crear y destruir.
      Desventajas: Aunque están aislados a nivel de procesos, no son tan seguros como las máquinas virtuales, ya que comparten el mismo kernel del sistema operativo anfitrión.
  
  3. Entornos de Pruebas en la Nube
  
      Descripción: Servicios como AWS, Google Cloud, o Azure permiten crear entornos virtualizados rápidamente donde puedes probar código sin afectar tu máquina local. Puedes configurar máquinas virtuales o usar servicios gestionados.
      Ventajas: Acceso a recursos casi ilimitados, no necesitas infraestructura local; es posible escalar según las necesidades.
      Desventajas: Costos asociados al uso de recursos en la nube; puede ser más lento dependiendo de la conexión a internet.
  
  4. Entornos de Pruebas Locales con Chroot (Linux)
  
      Descripción: chroot es una herramienta de Unix que cambia el directorio raíz de un proceso. Esto puede proporcionar un aislamiento básico del entorno para ejecutar programas, aunque el aislamiento no es tan completo como el de las máquinas virtuales.
      Ventajas: Es liviano y fácil de configurar en sistemas Unix/Linux; permite tener un entorno controlado.
      Desventajas: No es completamente seguro, ya que los procesos dentro de un chroot pueden acceder a recursos compartidos del sistema.
  
  5. Sandboxes en Sistemas Operativos (Windows Sandbox, macOS App Sandbox)
  
      Windows Sandbox: En sistemas Windows 10 y 11 Pro o Enterprise, puedes utilizar "Windows Sandbox", una funcionalidad que crea un entorno temporal aislado en el que puedes ejecutar programas de manera segura.
      macOS App Sandbox: macOS permite a los desarrolladores usar un modelo de caja de arena para las aplicaciones, restringiendo el acceso a recursos sensibles del sistema operativo.
      Ventajas: Integración nativa con el sistema operativo; configuración sencilla para escenarios comunes.
      Desventajas: Generalmente limitado a casos específicos (por ejemplo, solo Windows o macOS); en algunos casos, los recursos son limitados o no tan flexibles como una VM.
  
  6. Herramientas de Análisis de Seguridad (Sandboxing para Malware)
  
      Ejemplos: Cuckoo Sandbox, Any.Run, Hybrid Analysis.
      Descripción: Son entornos diseñados para ejecutar y analizar código sospechoso o malicioso de manera segura. Pueden ejecutarse en máquinas virtuales o contenedores, y tienen integradas herramientas de monitoreo para estudiar el comportamiento del código.
      Ventajas: Especializados en la detección y análisis de malware; proporcionan reportes detallados del comportamiento del código.
      Desventajas: Generalmente se enfocan en malware, por lo que puede no ser ideal para código no malicioso, aunque muchos soportan análisis generales.
  
  7. Entornos de Contención con SELinux/AppArmor
  
      Descripción: SELinux (Security-Enhanced Linux) y AppArmor son sistemas de control de acceso obligatorio (MAC) que puedes usar para crear políticas de seguridad y aislamiento para procesos específicos en sistemas Linux.
      Ventajas: Aislamiento a nivel de sistema, robustez en términos de seguridad, y control granular sobre los permisos de acceso.
      Desventajas: Requiere configuración avanzada y una buena comprensión de las políticas de seguridad; puede ser complicado de gestionar en un entorno de desarrollo.
  
  8. Emuladores
  
      Descripción: Para ciertos tipos de programas (por ejemplo, aplicaciones móviles), puedes usar emuladores como Android Emulator o QEMU para simular un entorno completo en tu máquina de desarrollo.
      Ventajas: Permite probar aplicaciones específicas sin hardware físico. Es útil para pruebas de dispositivos móviles o arquitecturas específicas.
      Desventajas: La emulación puede ser más lenta que ejecutar el código en un dispositivo real; no es una solución para todos los tipos de software.
  
  9. Aislamiento con Virtualización de Aplicaciones
  
      Descripción: Herramientas como Firejail (en Linux) o Cameyo (en Windows) permiten ejecutar aplicaciones en entornos aislados, limitando su acceso a los recursos del sistema operativo.
      Ventajas: Fácil de usar y configuraciones específicas para cada aplicación.
      Desventajas: Menos robusto en comparación con las soluciones de virtualización completas.
  
  Crea el entorno controlado y prueba la aplicación en él.

  
  Documenta cómo has desarrollado el proyecto en github.

  

En la plataforma: pega el enlace y y sube el repositorio comprimido.

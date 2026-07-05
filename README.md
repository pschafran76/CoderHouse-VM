1 Captura de pantalla.
<img width="1920" height="1080" alt="Captura de pantalla_20260705_123131" src="https://github.com/user-attachments/assets/8daa1b9b-bda2-4db7-84e5-ce414ec767b2" />


2 Justificación técnica: Explica en un párrafo por qué elegiste ese modo de red (Interna o Solo-Anfitrión) y por qué no usaste el modo "Puente" (Bridged).
   
Se recomienda utilizar el modo de red Interna o Solo-Anfitrión (Host-Only) en una máquina virtual de VirtualBox cuando el objetivo principal es mantener un entorno aislado, seguro y controlado. Estos modos permiten que la máquina virtual se comunique entre sí o con el sistema anfitrión sin exponerla directamente a la red física local. El modo Interna es ideal para crear una red privada entre varias máquinas virtuales sin que tengan acceso a internet ni a la red del anfitrión, mientras que el modo Solo-Anfitrión permite que las VMs se comuniquen con el host y entre ellas, pero sin visibilidad desde otros dispositivos de la red local.
No se recomienda el modo Puente (Bridged) porque este asigna una dirección IP real de la red física al equipo virtual, haciendo que aparezca como un dispositivo más en la red local. Esto aumenta significativamente la superficie de ataque (exponiendo la VM a posibles escaneos, ataques o accesos no deseados desde otros equipos), consume direcciones IP de la red real y puede generar problemas de seguridad o políticas de red en entornos corporativos o de laboratorio. En escenarios de pruebas, aprendizaje o desarrollo, el aislamiento ofrecido por Interna o Solo-Anfitrión es mucho más adecuado y seguro.   


3 Captura de pantalla del administrador de Instantáneas mostrando tu primer snapshot.
<img width="1920" height="1080" alt="Captura de pantalla_20260705_123435" src="https://github.com/user-attachments/assets/90cb2461-2150-4a38-b3ee-8a26f15c2d20" />

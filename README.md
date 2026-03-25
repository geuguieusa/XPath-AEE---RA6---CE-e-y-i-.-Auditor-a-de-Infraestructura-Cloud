* **¿Cuántas líneas de código habéis ahorrado al usar grupos?**
El esquema utiliza xs:group y xs:attributeGroup para centralizar definiciones comunes, y aunque hoy se usen una vez, permiten añadir nuevos elementos como <router> o <firewall> al instante sin repetir código, también cualquier cambio en la estructura global se refleja automáticamente en todos los componentes, eliminando la redundancia y facilitando el crecimiento de TechNova Cloud.

* **¿Qué error os da VS Code si intentáis poner dos servidores con el mismo ID?**
El esquema implementa la restricción <xs:unique> para garantizar que no existan IDs duplicados, entoces si intentas asignar el mismo ID a dos servidores, el validador mostrará el error cvc-identity-constraint.4.1 y saldrá de mensaje: > Duplicate unique value [ID_REPETIDO] declared for identity constraint "UnicoID"...

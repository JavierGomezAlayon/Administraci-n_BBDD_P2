# Administración_BBDD_P2
<img width="1113" height="441" alt="Practica 2 drawio" src="https://github.com/user-attachments/assets/6b4111c1-7a93-43a2-9198-f42793283c11" />


## Explicación de las entidades
En este apartado se recoge una breve descripción de las entidades definidas y además el rango y ejemplos de sus atributos
- **Cliente**: Persona que haya realizado al menos una compra.
  - Código (secuencial): Atributo identificativo que consiste en un código serial. : 1234
  - Crédito (bool): Indica si el cliente es con crédito o no. : true
    - **Cliente sin crédito**
    - **Cliente con crédito**
      - Datos bancarios (Objeto): Objeto que recoge todos los datos bancarios del cliente con crédito. : (no sé como representar un objeto)
        - Número (varchar): Número de la cuenta bancaria. : ES91 2100 0418 4502 0005 1332
        - Entidad (varchar): Entidad de la cuenta bancaria. : CaixaBank
        - Sucursal (varchar): Sucursal en la que está la cuenta bancaria. : 0418 – Rambla Santa Cruz (Tenerife)
- **Farmacia**: Sitio donde se pueden comprar medicamentos, donde se almacenan y en algunos casos donde se producen medicamentos
  - Código (secuencial): Atributo identificativo que consiste en un código serial. : 3891
- **Laboratorio**: Sitio donde se fabrican medicamentos pero no los venden.
  - Código (secuencial): Atributo identificativo que consiste en un código serial. : 0001
  - Teléfono (Integer): Número telefónico del laboratorio. : 645389283098
  - Nombre (varchar): Nombre del laboratorio. : Fixer
  - Fax (varchar): Número (con las barras) del fax. : 555-123-4567
  - Dirección postal (varchar): Dirección postal del laboratorio. : 65204
  - Nombre persona de contacto (varchar): Nombre de la persona de contacto que tiene el laboratorio. : Juan García Alla
- **Medicamento**: 
  - Código (secuencial): Atributo identificativo que consiste en un código serial. : 1003
  - Tipo (varchar): Tipo de medicamento. : Jarabe
  - Libre (bool): Si el medicamento se puede comprar sin receta o nó. : true
  - Nombre (varchar): Nombre del medicamento. : Paracetamol
  - Precio (Number): Precio de compra del medicamento. : 15,5
  - Vendidas (Integer): Unidades vendidas de dicho medicamento. : 120
- **Familia**
  - Código (secuencial): Atributo identificativo que consiste en un código serial. : 4550
  - Enfermedades aplicables (varchar): Nombre de las enfermedades que combate los medicamentos de dicha familia. : Gripe
## Explicación de las relaciones
Aquí se explica las relaciones definidas.
- **Compra**
  - Fecha compra
  - Número
  - Fecha pago (solo si el comprador es un cliente con crédito)
- **Almacena**
  - Reserva
- **Fabricación** 
- **Obtención**
- **Pertenece**

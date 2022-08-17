CREACIONES DE LAS TABLAS DETALLES
====================================
create table detalle_cli_pizz(
idCliente int NOT NULL,
idPizza int NOT NULL,
FOREIGN KEY(idCliente ) REFERENCES clientes( idCliente ),
FOREIGN KEY(idPizza ) REFERENCES pizzas (idPizza )
);

create table detalle_pizz_pza(
idPizza int NOT NULL,
idPizeria int NOT NULL,
FOREIGN KEY(idPizza ) REFERENCES pizzas( idPizza ),
FOREIGN KEY(idPizeria ) REFERENCES pizeria (idPizeria )
);

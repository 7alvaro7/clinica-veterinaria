📖 Escenario

Una clínica veterinaria gestiona un máximo de 25 mascotas registradas en su sistema.

Cada mascota está identificada mediante un id único y dispone de la siguiente información:

id (int)
nombre (String)
especie (String)
edad (int)

El sistema debe permitir registrar mascotas, buscarlas, mostrarlas y contar cuántas están actualmente almacenadas.

Recuerda crear los commits adecuados según vas desarrollando la solución.

🧩 Requisitos técnicos

1️⃣ Clase Mascota

Debe incluir:

Atributos privados.
Constructor completo.
Métodos getters.
Método toString().

Javadoc en:

Clase
Constructor
Métodos públicos

2️⃣ Clase ClinicaVeterinaria

Debe incluir:

Atributos:

private Mascota[] mascotas;
private final int NUM_MAX_MASCOTAS;

Constructor:

Asegúrate de que el número máximo de mascotas recibido sea positivo.

Métodos obligatorios:

public Mascota buscarMascota(int id)
private int buscarPrimerHuecoLibre()
public boolean registrarMascota(Mascota mascota)
public String mostrarMascotas()
public int contarMascotas()

🔍 Comportamiento esperado

buscarMascota(int id)

Devuelve la mascota con ese id.
Devuelve null si no existe.

buscarPrimerHuecoLibre()

Devuelve la primera posición null.
Devuelve -1 si el array está completo.

registrarMascota(Mascota mascota)

Solo añade si no existe otra con el mismo id.
Solo añade si hay hueco disponible.
Devuelve true si se añade.
Devuelve false si no puede añadirse.

mostrarMascotas()

Devuelve el listado de mascotas con su información.

contarMascotas()

Devuelve el número real de mascotas almacenadas.

🖥 Clase Main

Debe:

Crear una ClinicaVeterinaria con capacidad para 25 mascotas.
Registrar al menos 3 mascotas.
Mostrar mascotas.
Mostrar el total almacenado.
Probar una búsqueda existente y otra inexistente.

📊 Criterios de evaluación

Criterio | Peso
Diseño correcto de clases | 20%
Encapsulación adecuada | 10%
Uso correcto del array fijo | 20%
Método registrarMascota correcto | 15%
Recorrido y visualización correctos | 10%
Conteo correcto | 10%
Javadoc adecuado | 10%
Orden y claridad del código | 5%

⚠️ Errores frecuentes a evitar

No inicializar el array en el constructor.
Usar ArrayList.
No comprobar null antes de acceder a un objeto.
Sobrescribir posiciones ocupadas.
No devolver false cuando el sistema está lleno.
No documentar correctamente.
Hacer atributos públicos.

📌 Entrega

Proyecto completo.
Código funcional.
Compila sin errores.
Nombres claros y coherentes.

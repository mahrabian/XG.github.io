






<!DOCTYPE html>
<html>
<head>
    <link rel="stylesheet" type="text/css" href="estilos/index.css">
    <link rel="icon" href="img/favicon.ico" type="image/x-icon">
    <title>XG/Inicio</title>
	<style>
	/* Estilos para botones */
.button {
    
    padding: 10px;
    border: 1px solid #4cd137;
    border-radius: 4px;
    box-sizing: border-box;
    background-color: #4cd137;
    color: white;
    cursor: pointer;
    transition: background-color 0.3s ease, border-color 0.3s ease;
}

.button:hover {
    background-color: #45a049;
    border-color: #45a049;
}

.button:active {
    transform: scale(0.95);
}
	</style>
</head>
<body>
    <center><img src="img/XG.png" width="468" height="178" alt=""/></center>
        
    <div class="content">
        <!-- Cliente -->
        <div class="dropdown">
            <span>Clientes</span>
            <div class="dropdown-content">
                <a href="agregar_cliente.php">Cargar</a>
                <a href="mostrar_clientes.php">Ver</a>
				<a href="mostrar_clientes_suspendidos.php">Ver Suspendidos</a>
                <!-- Puedes añadir más elementos de menú aquí -->
            </div>
        </div>
        <!-- Rutinas -->
        <div class="dropdown">
            <span>Rutinas</span>
            <div class="dropdown-content">
                <a href="cargar_rutina_basica.php">Cargar</a>
                <a href="mostrar_rutinas_basicas.php">Ver</a>
                <!-- Puedes añadir más elementos de menú aquí -->
            </div>
        </div>
        <!-- Planes -->
        <div class="dropdown">
            <span>Planes</span>
            <div class="dropdown-content">
                <a href="cargar_planes.php">Cargar</a>
                <a href="mostrar_planes.php">Ver</a>
                <!-- Puedes añadir más elementos de menú aquí -->
            </div>
        </div>
        <!-- Ejercicios -->
        <div class="dropdown">
            <span>Ejercicios</span>
            <div class="dropdown-content">
                <a href="cargar_ejercicio.php">Cargar</a>
                <a href="mostrar_ejercicios.php">Ver</a>
                <!-- Puedes añadir más elementos de menú aquí -->
            </div>
        </div>
		<div class="dropdown">
            <span>Asistencia</span>
            <div class="dropdown-content">
                <a href="registro_asistencia.php">Cargar</a>
                <a href="mostrar_asistencia.php">Ver</a>
                <!-- Puedes añadir más elementos de menú aquí -->
            </div>
        </div>
		<div class="dropdown">
            <span>Estadisticas</span>
            <div class="dropdown-content">
                <a href="estadisticas.php">Ver</a>
            </div>
        </div>
		
		<div class="dropdown">
            <span>Recaudacion</span>
            <div class="dropdown-content">
				 <a href="login.php">Login</a>
                <a href="register.php">Registrarse</a>
            </div>
        </div>
		
           
           
				 <input type="button" class="button" value="Tienda" onclick="window.location.href='index_tienda.php';">
            
       
		
		
		
		 <?php
    // Configuración de conexión a la base de datos
    $host = 'localhost';
    $usuario = 'root';
    $contr = 'LJEM37788502';
    $base_datos = 'xg';

    // Conexión a la base de datos
    $conexion = new mysqli($host, $usuario, $contr, $base_datos);
    if ($conexion->connect_error) {
        die('Error al conectar a la base de datos: ' . $conexion->connect_error);
    }

    // Obtener fecha actual en formato compatible con MySQL
    $hoy = date('Y-m-d');

    // Consulta SQL para obtener clientes con cuota vencida usando JOIN
    $sql_clientes_cuota_vencida = "SELECT clientes.id_cliente, clientes.nombre, clientes.apellido FROM clientes JOIN cuotas ON clientes.id_cliente = cuotas.id_cliente WHERE cuotas.fecha_vencimiento <= '$hoy' and activo = 1 ORDER BY clientes.apellido, clientes.nombre ASC ";
    
    // Ejecutar la consulta
    $result_clientes_cuota_vencida = $conexion->query($sql_clientes_cuota_vencida);

    // Verificar si la consulta fue exitosa
    if (!$result_clientes_cuota_vencida) {
        // Mostrar mensaje de error si la consulta falla
        echo 'Error en la consulta SQL: ' . $conexion->error;
    } else {
        // Verificar si hay resultados
if ($result_clientes_cuota_vencida->num_rows > 0) {
    // Iniciar la etiqueta del menú desplegable
    echo '<center>'; 
    echo '<select id="clientesDeudores" onchange="verDetalleCliente(this.value)">';
    echo '<option value="">Cuotas vencidas</option>';
    // Mostrar enlaces para los clientes con cuota vencida como opciones del menú desplegable
   	
	

while ($row = $result_clientes_cuota_vencida->fetch_assoc()) {
    $id_cliente = $row['id_cliente'];
    $nombre = $row['nombre'];
    $apellido = $row['apellido'];
    $nombre_cliente = $row['nombre'] . ' ' . $row['apellido'];
    echo "<option value='$id_cliente'>$nombre_cliente</option>";
}

// Cerrar la etiqueta del menú desplegable
echo '</select>';
echo '</center>';
}

// JavaScript para redireccionar al detalle del cliente seleccionado
echo '<script>
    function verDetalleCliente() {
        // Obtener el valor seleccionado del menú desplegable
        var selectedId = document.getElementById("clientesDeudores").value;

        // Redireccionar a la página con los parámetros
        window.location.href = "mostrar_membresia.php?id_cliente=" + selectedId;
    }
</script>';

	}
		

    // Calcular la fecha de vencimiento en 1 día
    $aviso_vencimiento_1_dia = date('Y-m-d', strtotime('+1 day'));

    // Consulta SQL para obtener clientes con cuota por vencer en 1 día
    $sql_clientes_cuota_por_vencer_1_dia = "SELECT clientes.id_cliente, clientes.nombre, clientes.apellido FROM clientes JOIN cuotas ON clientes.id_cliente = cuotas.id_cliente WHERE cuotas.fecha_vencimiento = '$aviso_vencimiento_1_dia' and activo = 1 ORDER BY clientes.apellido, clientes.nombre ASC ";

    // Ejecutar la consulta
    $result_clientes_cuota_por_vencer_1_dia = $conexion->query($sql_clientes_cuota_por_vencer_1_dia);

    // Verificar si la consulta fue exitosa
    if (!$result_clientes_cuota_por_vencer_1_dia) {
        // Mostrar mensaje de error si la consulta falla
        echo 'Error en la consulta SQL: ' . $conexion->error;
    } else {
        // Verificar si hay resultados
        if ($result_clientes_cuota_por_vencer_1_dia->num_rows > 0) {
            // Iniciar la etiqueta del menú desplegable
           echo '<center>';
            echo '<select id="clientesPorVencer1Dia" onchange="verDetalleCliente(this.value)">';
            echo '<option value="">Cuotas por vencer en 1 día</option>';
            // Mostrar enlaces para los clientes con cuota por vencer en 1 día como opciones del menú desplegable
            while ($row = $result_clientes_cuota_por_vencer_1_dia->fetch_assoc()) {
                $id_cliente = $row['id_cliente'];
				$nombre = $row['nombre'];
				$apellido = $row['apellido'];
                $nombre_cliente = $row['nombre'] . ' ' . $row['apellido'];
                echo "<option value='$id_cliente'>$nombre_cliente</option>";
            }
            // Cerrar la etiqueta del menú desplegable
            echo '</select>';
            echo '</center>';
        }
    }

    // Calcular la fecha de vencimiento en 2 días
    $aviso_vencimiento_2_dias = date('Y-m-d', strtotime('+2 days'));

    // Consulta SQL para obtener clientes con cuota por vencer en 2 días
    $sql_clientes_cuota_por_vencer_2_dias = "SELECT clientes.id_cliente, clientes.nombre, clientes.apellido FROM clientes JOIN cuotas ON clientes.id_cliente = cuotas.id_cliente WHERE cuotas.fecha_vencimiento = '$aviso_vencimiento_2_dias' and activo = 1 ORDER BY clientes.apellido, clientes.nombre ASC ";

    // Ejecutar la consulta
    $result_clientes_cuota_por_vencer_2_dias = $conexion->query($sql_clientes_cuota_por_vencer_2_dias);

    // Verificar si la consulta fue exitosa
    if (!$result_clientes_cuota_por_vencer_2_dias) {
        // Mostrar mensaje de error si la consulta falla
        echo 'Error en la consulta SQL: ' . $conexion->error;
    } else {
        // Verificar si hay resultados
        if ($result_clientes_cuota_por_vencer_2_dias->num_rows > 0) {
            // Iniciar la etiqueta del menú desplegable
            echo '<center>';
            echo '<select id="clientesPorVencer2Dias" onchange="verDetalleCliente(this.value)">';
            echo '<option value="">Cuotas por vencer en 2 días</option>';
            // Mostrar enlaces para los clientes con cuota por vencer en 2 días como opciones del menú desplegable
            while ($row = $result_clientes_cuota_por_vencer_2_dias->fetch_assoc()) {
                $id_cliente = $row['id_cliente'];
				$nombre = $row['nombre'];
    			$apellido = $row['apellido'];
                $nombre_cliente = $row['nombre'] . ' ' . $row['apellido'];
                echo "<option value='$id_cliente'>$nombre_cliente</option>";
            }
            // Cerrar la etiqueta del menú desplegable
            echo '</select>';
            echo '</center>';
        }
    }

    // JavaScript para redireccionar al detalle del cliente seleccionado
   echo '<script>
    function verDetalleCliente(id_cliente, nombre, apellido) {
        if (id_cliente !== "") {
            var url = "mostrar_membresia.php?id_cliente=" + id_cliente + "&nombre=" + encodeURIComponent(nombre) + "&apellido=" + encodeURIComponent(apellido);
            window.location.href = url;
        }
    }
</script>';
echo '<p>';
		// Consulta SQL para verificar si un cliente no ha tenido asistencias registradas en los últimos 30 días
$sqlClienteSinAsistencias = "SELECT id_cliente, nombre, apellido FROM clientes WHERE fecha_inicio <= DATE_SUB(NOW(), INTERVAL 7 DAY) AND NOT EXISTS (
    SELECT * FROM asistencias WHERE asistencias.id_cliente = clientes.id_cliente AND fecha >= DATE_SUB(NOW(), INTERVAL 10 DAY)
) AND activo = 1";

// Ejecutar la consulta
$resultClienteSinAsistencias = $conexion->query($sqlClienteSinAsistencias);

// Verificar si la consulta fue exitosa
if (!$resultClienteSinAsistencias) {
    // Mostrar mensaje de error si la consulta falla
    echo 'Error en la consulta SQL: ' . $conexion->error;
} else {
           
		// Imprimir un formulario con un botón si hay clientes sin asistencias
if ($resultClienteSinAsistencias->num_rows > 0) {
    echo '<form action="clientes_ausentes.php" method="GET">';
    echo '<input type="submit" class="button" value="Ver clientes ausentes">';
    echo '</form>';


    }
}
  
    // Cerrar la conexión a la base de datos
    $conexion->close();
    ?>
		

   		
	
        
        <h6><a style='position: fixed; bottom: 0; left: 0;' href="copia_seguridad.php">Realizar Backup</a></h6>
    
		
</body>
</html>

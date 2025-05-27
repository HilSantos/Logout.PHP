# Logout.PHP
Criação da pagina de logout.php

<?php
include('segurancazero.php');
session_destroy();
header('Location: index.php');
exit();

?>

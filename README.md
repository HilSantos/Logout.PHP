# Logout.PHP
Criação da pagina de logout.php

<?php
// Inclui o arquivo de segurança para garantir que apenas usuários autenticados possam acessar //
include('segurancazero.php');

// Encerra a sessão do usuário, removendo todos os dados da sessão //
session_start();
session_destroy();

// Redireciona o usuário para a página inicial após o logout //
header('Location: index.php');
exit();
?>

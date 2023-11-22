conserte esse codigo $stmt = $mysqli->prepare("SELECT idAgendamento, idServico, idFuncionario, nomeCliente, sobrenomeCliente, data_consulta, horario_consulta FROM Agendamento WHERE idCliente = ?");
$stmt->bind_param("i", $idCliente); com base nesse banco de dados CREATE TABLE IF NOT EXISTS Agendamento (
    idAgendamento INT AUTO_INCREMENT PRIMARY KEY,
    idServico INT NOT NULL,
    idFuncionario INT NOT NULL,
    nomeCliente VARCHAR(100) NOT NULL,
    sobrenomeCliente VARCHAR(100) NOT NULL,
    data_consulta DATE NOT NULL,
    horario_consulta TIME NOT NULL,
    FOREIGN KEY (idServico) REFERENCES Servico(idServico),
    FOREIGN KEY (idFuncionario) REFERENCES Funcionario(idFuncionario)
);

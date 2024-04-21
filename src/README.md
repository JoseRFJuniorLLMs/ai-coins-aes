# Introduction

Criptografia de Arquivos de Backup: Independentemente da opção escolhida, certifique-se de criptografar os arquivos de backup para garantir a segurança das informações. Você pode usar algoritmos de criptografia robustos, como AES (Advanced Encryption Standard), para isso.

Chave privada:
id: Identificador único da chave privada.
chave_privada: A própria chave privada, que deve ser armazenada de forma segura e criptografada.
usuario_id: Identificador do usuário proprietário da chave privada.
Endereço da carteira:
id: Identificador único do endereço da carteira.
endereco: Endereço público da carteira de criptomoeda.
usuario_id: Identificador do usuário associado à carteira.
Dados da transação:
id: Identificador único da transação.
valor: Valor da transação em criptomoeda.
endereco_destino: Endereço de destino para a transação.
hash_transacao: Hash único que identifica a transação.
data_hora: Data e hora da transação.
usuario_id: Identificador do usuário que realizou a transação.
Histórico de transações:
Para manter o histórico de transações, podemos usar uma tabela separada ou simplesmente adicionar um campo transacoes na tabela de endereços da carteira. Aqui, vamos optar por uma tabela separada.
id: Identificador único do histórico de transações.
endereco_id: Identificador do endereço da carteira associado à transação.
transacao_id: Identificador da transação associada ao histórico.
tipo: Tipo de transação (enviada ou recebida).
Dados de autenticação e segurança:
id: Identificador único do usuário.
nome_usuario: Nome de usuário.
senha: Hash de senha ou senha criptografada.
autenticacao_2fa: Chave secreta para autenticação de dois fatores (opcional).
salt: Valor aleatório para aumentar a segurança da senha (se estiver usando hash de senha).
Metadados adicionais:
id: Identificador único do metadado adicional.
transacao_id: Identificador da transação associada ao metadado.
remetente: Remetente da transação.
destinatario: Destinatário da transação.
categoria: Categoria da transação (opcional).
nota: Nota ou mensagem associada à transação (opcional).

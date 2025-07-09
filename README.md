# CaseIU

O arquivo Alunos.csv original possui erro de formato de dados na última linha que exiguiu correção:
aluno_id,nome,turma,escola_id
101,Ana Ferreira,6¼ A,201
102,Bruno Lima,6¼ A,201
"103,Carla Menezes,6¼ B;202"

Ficou assim:
aluno_id,nome,turma,escola_id
101,Ana Ferreira,6¼ A,201
102,Bruno Lima,6¼ A,201
103,Carla Menezes,6¼ B,202

O código foi gerado através do Gemini do Google Colab através do seguinte prompt:
O arquivo Alunos.csv possui as seguintes colunas: aluno_id, nome, turma, escola_id
O arquivo Testes.csv possui as seguntes colunas: aluno_id, disciplina, nota, bimestre
Crie um código que una as duas tabelas através dos campos aluno_id e armazene na tabela AlunosxTestes com os seguintes campos: aluno_id, nome, turma, disciplina, nota, bimestre.
Ordene a tabela AlunosxTestes pelos campos turma em ordem crescente e nome em ordem crescente.
Salve a tabela AlunosxTestes no arquivo alunos_avaliacoes.csv

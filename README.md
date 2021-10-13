Mensagem: "<saudação>, bem-vindo a UFC!"  
1. A saudação é:  
	- “Bom dia!”, se o horário for de 08-12h;  
	- “Boa tarde!”, se o horário for de 12-18h;  
	- “Boa noite!”, se o horário for de 18-22h;  
2. Se a ligação for recebida fora do horário acima, faça:  
	○ Mensagem: “O horário de atendimento é de 08 às 22h”;  
	○ Desliga.  
3. Caso a ligação seja recebida dentro do horário de atendimento, apresente as opções:  
	- Mensagem: "Se você é aluno, digite 1. Se você é administrador, digite 2. Para repetir esta mensagem, digite 0".  
	- Caso 1:  
		- Mensagem: "Para consultar matrícula, digite 1. Para falar com a recepção do campus, digite 2. Para retornar ao menu principal, digite 3."  
		- Caso 1.1:  
			 Mensagem: "Digite o número de matrícula:"  
			b. Na tela do Asterisk deverá aparecer a matrícula digitada (NoOp).  
			c. EXTRA:  
				● Verificar se matrícula digitada está armazenada dentro de um banco de dados.  
				● Caso sim:  
					○ Mensagem: "Aluno matriculado!”  
				● Caso não:  
					○ Mensagem: "Aluno não matriculado!"  
					○ Desliga.  
		➢ Caso 1.2:  
			a. Mensagem: "Sua ligação está sendo transferida para a recepção."  
			b. Transfere a ligação para o número 100.  
		➢ Caso 1.3:  
			a. Retorna para o menu principal.  
		➢ Opção Inválida:  
			a. Mensagem: “Opção inválida. Por favor, digite novamente.”  
			b. Retorna para o “Caso 1”.  
	ii. Caso 2:  
		■ Mensagem: "Digite a senha de administrador e ao final digite #."  
		■ Se a senha digitada for válida (Senha: “987123654”):  
			➢ Mensagem: "Olá administrador! Para falar com a direção, digite 1. Para falar com a TI, digite 2. Para fazer uma ligação externa, digite 3. Para reiniciar o servidor, digite 4. Para retornar ao menu principal, digite 5."  
		➢ Caso 2.1:  
			a. Mensagem: "Sua ligação está sendo transferida para a direção."  
			b. Transfere a ligação para o número 200.  
		➢ Caso 2.2:  
			a. Mensagem: "Sua ligação está sendo transferida para a TI."  
			b. Transfere a ligação para o número 300.  
		➢ Caso 2.3:  
			a. Mensagem: "Digite o número que deseja ligar e ao final, aperte #."  
			b. Transfere a ligação para o número digitado.  
		➢ Caso 2.4:  
			a. Mostra mensagem no Asterisk: "Reiniciando o servidor"  
		i. Caso 2.5:  
			■ Retorna ao menu principal.  
		ii. Opção Inválida:  
			■ Mensagem: "Opção inválida. Por favor, digite novamente"  
			■ Retorna para o "Caso 2".  
		★ Caso contrário:
			a. Mensagem: "Senha incorreta!"  
			b. Desliga.  
	iii. Caso 0:  
		■ Repete opções.  
	iv. Opção Inválida:  
		■ Mensagem: "Opção inválida. Por favor, digite novamente."  
		■ Retorna para o Menu Principal.  

# Simple-Menu
Code IN C++
Menu simples com interface de usuario login e senha, e opcoes na aba principal!

#include <iostream>
#include <string>

using namespace std;

int main() {
	int senha, login, op, op1, soma, sub, div, mult, pass, log;
	float v1, v2;
	cout << "Deseja fazer login(opcao1) ou se cadastrar(opcao2) :";
	cin >> op1;
	while(op1 != 1 && op1 !=2)
	{	
	cout << "Opcao Invalida, Deseja fazer login(opcao1) ou se cadastrar(opcao2) :";
				cin >> op1;
	}
	switch(op1){
	case 1:
	cout << "Login:";
	 cin >> login;
	 while(login != 1234){
		 	cout << "Login incorreto, Digite denovo:";
		 	 cin >> login;
		 }
	 	if(login == 1234){
	 		cout << "Senha:";
	 		 cin >> senha;
		 }
		 while(senha != 9999){
		 	cout << "Senha incorreta, Digite denovo:";
		 	 cin >> senha;
		 }	 
	break;
	
	case 2:
		cout << "Digite o LOGIN que deseja utilizar (somente numeros):";
		cin >> log;
		cout << "Digite a SENHA que deseja utilizar (somente numeros):";
		cin >> pass;
			cout << "Cadastro realizado com sucesso!\n";
	cout << "Login:";
	 cin >> login;
	 while(login != 1234 && login != log){
		 	cout << "Login incorreto, Digite denovo:";
		 	 cin >> login;
		 }
	 	 
		 while(senha != 9999 && senha != pass){
		 	cout << "Senha:";
		 	 cin >> senha;
		 }
						
	break;
}	
	if(senha == 9999 || senha == pass)
	{
		 	cout << "Acesso Permitido!\n";
		 
		 cout << "Voce acaba de entrar na aba principal, escolha uma opcao a seguir!\n";	
		  cout << "1-soma\n2-subtracao\n3-divisao\n4-multiplicacao\n";
		   cout << "Escolha uma opcao:";
		   cin >> op;
	 while(op != 1 && op != 2 && op != 3 && op != 4){
	 	cout << "Opcao invalida, Digite uma opcao validavel:";
	 	 cin >> op;
	 }
		if(op == 1){
			cout << "Voce escolheu soma!\n";
			cout << "digite o primeiro e o segundo valor: ";
			cin >> v1 >> v2;
				soma = v1 + v2;
			cout << v1 << "+" << v2 << "=" << soma;		
		}
		if(op == 2){
			cout << "Voce escolheu subtracao!\n";
			cout << "digite o primeiro e o segundo valor: ";
			cin >> v1 >> v2;
				sub = v1 - v2;
			cout << v1 << "-" << v2 << "=" << soma;	
		}
		if(op == 3){
			cout << "Voce escolheu divisao!\n";
			cout << "digite o primeiro e o segundo valor: ";
			cin >> v1 >> v2;
			cout << v1 << "/" << v2 << "=" << soma;	
		}
		if(op == 4){
			cout << "Voce escolheu multiplicacao!\n";
			cout << "digite o primeiro e o segundo valor: ";
			cin >> v1 >> v2;
			cout << v1 << "*" << v2 << "=" << soma;
		}
	}
	return 0;
}


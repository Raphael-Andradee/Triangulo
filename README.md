# Triangulo

#include<iostream>
using namespace std;



int main() {

	int continuar = 1;


	float a, b, c;

	do { // comando dentro do (do) // exibir menu

		cout << "Menu\n\n";

		cout << "Verificar tipo de triangulo\n\n";

		cout << "Indique:\n\n 1 para continuar \n\n 2 para sair.\n\n";

		cin >> continuar;

		if (continuar == 1) {

		cout << " Indique o a medida dos 3 lados do triangulo:\n";

		

			cout << " Indique 1º valor:\n\n";

			cin >> a;

			cout << " Indique 2º valor:\n\n";

			cin >> b;

			cout << " Indique 3º valor:\n\n";

			cin >> c;

			if (a == b && b == c) //  atento aos parentesis e o simbolo && 
			{
				cout << " Este triângulo é equilatero\n";
			}
			else if (a == b && b != c)
			{
				cout << " Este triângulo é isócele\n";
			}
			else if (a != b && b != c)
			{
				cout << " Este triângulo é escaleno\n";
			}
			else if (a != b && b == c)
			{
				cout << " Este triângulo é isócele\n";
			}
			else if (c == a && a != b)
			{
				cout << " Este triângulo é isócele\n";
			}

			

		}

		
	}
		while (continuar != 2); // O loop continua até o usuário escolher sair
	     cout << "Saindo do programa..";

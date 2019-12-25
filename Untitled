#include <iostream>
#include <cstring>
#include <vector>
using namespace std;

string command = "";


void oi() { //о программе
	cout << "--------------------------------------" << endl;
	cout << "Версия windows 7, х64 bit\n"
		<< "Создано ArlCloud\n"
		<< "Месторасположение файла \n";
	cout << "--------------------------------------" << endl;
}
void clea() { //очистка
	cout << "Очистка" << endl;
	system("cls");
	cout << "Чтобы пользоваться меню снова наберите /*men.tr" << endl;
	
 }

void passur() { //смена пароля
	//сделать
}

void exsi() { //выход из программы
	cout << "Выход из программы..." << endl; //готово
	exit(EXIT_SUCCESS);
}

void spiso() { //список команд
	cout << "1. /*men.tr - вызвать меню.\n"
		<< "2. /*clr.tr - очистить консоль\n"
		<< "3. /*pas.ur - сменить пароль\n"              //готово
		<< "4. /*exs.mr - выйти\n"
		<< "5. /*ac.tr - посмотреть о программе\n"
		<< "6. /*ard.mr - удалить программу\n"
		<< "7. /*\n" << endl; //не задано
	
}

void deli() { //удалить программу

}

void func() {
	// Здесь будет функция
	int variant;
	cout << "Выберите функцию\n" << endl;
	cout << "1. Посмотреть данные о программе\n"
		<< "2. Удалить программу\n"
		<< "3. Ввести команды\n"
		<< "4. Сменить пароль\n"
		<< "5. Список команд\n"
		<< "6. Выход\n"
		<< "7. Очистка\n" << endl;
	cout << ">>> ";
	cin >> variant;
	///////////////////////Выбор программы по меню.
	switch (variant) {
	case 1:
		oi();
		cout << "Чтобы снова пользоваться меню наберите /*men.tr" << endl;				
		break;
	case 2:
		deli();
		break;
	case 3:
		//ввод
		break;
	case 4:
		cout << "Проль" << endl;
		break;
	case 5:
		spiso();
		break;	
	case 6:
		//выход
		exsi();
		break;
	case 7:
		clea();
		break;
	default:
		cerr << "Вы выбрали неверный вариант" << endl;
		exit(EXIT_FAILURE);
	}
	cout << ">>> ";
	cin >> command; //ожидаем команду после меню

	///////////////////////выбираем команду
	if (command == "/*men.tr") {
		func();
	}
	else if (command == "/*clr.tr") {
		clea();
	}
	else if (command == "/*pas.ur") {
		passur();
	}
	else if (command == "/*exs.mr") {
		exsi();
	}
	else if (command == "/*ac.tr") {
		spiso();
	}
	else if (command == "/*ard.mr") {
		deli();
	}
	else {

	}

}



int main(int argc, char* argv[]) {
	///////////////////////проверяем пароль
	setlocale(LC_ALL, "Rus"); 
	char password[32];
	char popytka = 0;

	while (1) {
		for (int i = 0; i < 32; i++)
			password[i] = ' ';

		cout << "Введите пароль: ";
		cin >> password;

		if (strcmp(password, "123") == 0) //Пароль
			break;
		else {
			popytka++;
			if (popytka == 3) {
				//если пароль не верный  3 раза
				cout << "Вы три раза неправильно ввели пароль. Обратитесь к администратору.\n";
				return 0;
			}
			//если пароль введён не верно 1-2 раза
			else if (popytka == 1) cout << "Неправильный пароль. Осталось две попытки.\n";
			else if (popytka == 2) cout << "Неправильный пароль. Осталась одна попытка.\n";
		}
	}
	cout << "Теперь вы в системе.\n";
	cout << "--------------------------------------" << endl;
	func();// если пароль правильный вызываем меню
}
# void main() {
  String nome = "tesoura";
  int idade = 16;
  double altura = 1.65;
  bool trabalho = true;


  print(
    "segunda nome $nome | idade $idade | altura : $altura | trabalho: $trabalho",
  );
}


2


void main() {
  int a = 17;
  int b = 5;


  print(a + b); //
  print(a - b);
  print(a * b); // multiplicacao
  print(a / b); // divisao com / double
  print(a ~/ b); // divisao inteira
  print(a % b); // resto da diversao
}


3


void main() {
  // ===== ENTRADAS =====
  double nota1 = 7.2;
  double nota2 = 8.0;
  double nota3 = 6.2;
  // ====================
  double media = (nota1 + nota2 + nota3) / 3;
  print('Média: $media');
}


4


void main() {
  int A = 5;
  int B = 9;
  int c = 0;


  print("$A, $B");


  c = A;
  A = B;
  B = c;


  print("$A, $B");
}


Início da citação direta


Enviada por Pedro Pepes de Campos
4
Fim da citação direta pressione a tecla L e inclua um link para a mensagem original
nao e 4 e 5


Pedro Pepes de Campos, qua. 14:12
6


void main() {
  List<int> numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  List<int> pares = [];
  List<int> impares = [];


  for (int numero in numeros) {
    if (numero % 2 == 0) {
      pares.add(numero);
    } else {
      impares.add(numero);
    }
  }


  print('Números pares: $pares');
  print('Números ímpares: $impares');
}


Pedro Pepes de Campos, qua. 14:15
7


void main() {


  List<int> numeros = [10, -5, 0, 23, -1, 0, 8, -42];


  
  List<int> positivos = [];
  List<int> negativos = [];
  List<int> zeros = [];


  
  for (int numero in numeros) {
    if (numero > 0) {
      positivos.add(numero);
    } else if (numero < 0) {
      negativos.add(numero);
    } else {
      zeros.add(numero);
    }
  }


 
  print('Positivos: $positivos');
  print('Negativos: $negativos');
  print('Zeros: $zeros (Quantidade: ${zeros.length})');
}


Pedro Pepes de Campos, qua. 14:36
void main() {
  int idade = 25;


  if (idade <= 12) {
    print('Criança');
  } else if (idade >= 12 && idade <= 17) {
    print('Adolescente');
  } else if (idade >= 18 && idade <= 59) {
    print('Adulto');
  } else if (idade >= 60) {
    print('Idoso');
  }
}


Você, qua. 14:43
void main() {
  double nota = 6.6;


  if (nota >= 7) {
    print('aprovado');
  } else if (nota >= 5 || nota <= 6.9) {
    print('recuperação');
  } else if (nota <= 5) {
    print('reprovado');
  }
}


Você, qua. 14:58
void main() {


  int totalMinutos = 200;


  if (totalMinutos < 0) {
    print('Valor inválido: os minutos não podem ser negativos.');
  } else {
    int horas = totalMinutos ~/ 60;
    int minutos = totalMinutos % 60;
    print('$horas h e $minutos min');
  }
}


Início da citação direta
Enviada por Você
void main() {


  int totalMinutos = 200;


  if (totalMinutos < 0) {
    print('Valor inválido: os minutos não podem ser negativos.');
  } else {
    int horas = totalMinutos ~/ 60;
    int minutos = totalMinutos % 60;
    print('$horas h e $minutos min');
  }
}
Fim da citação direta pressione a tecla L e inclua um link para a mensagem original
atividade 4


Você, qua. 15:01
atividade 10


void main() {
  // ===== ENTRADAS =====
  double n1 = 4;
  double n2 = 9;
  double n3 = 9;
  // ====================


  double maior = n1;


  if (n2 > maior) {
    maior = n2;
  }
  if (n3 > maior) {
    maior = n3;
  }


  print('Maior número: $maior');
}


void main() {
  
  int idade = 20;
  bool estudante = true;
  


  double valor = 40.0;


  if (idade < 0) {
    print('Idade inválida.');
  } else {
    if (idade < 12 || idade >= 60 || estudante) {
      valor = valor / 2;
    }
    print('Valor a pagar: R\$ ${valor.toStringAsFixed(2)}');
  }
}


11


void main() {
  // ===== ENTRADAS =====
  int ano = 2024;
  // ====================


  if (ano <= 0) {
    print('Ano inválido.');
  } else if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
    print('$ano é bissexto.');
  } else {
    print('$ano não é bissexto.');
  }
}


12


atividade 13
void main() {
  // ===== ENTRADAS =====
  double a = 5;
  double b = 5;
  double c = 8;
  // ====================


  if (a <= 0 || b <= 0 || c <= 0) {
    print('Valores inválidos: os lados devem ser maiores que zero.');
  } else if (a < b + c && b < a + c && c < a + b) {
    if (a == b && b == c) {
      print('Triângulo Equilátero');
    } else if (a == b || a == c || b == c) {
      print('Triângulo Isósceles');
    } else {
      print('Triângulo Escaleno');
    }
  } else {
    print('Os lados não formam um triângulo.');
  }
}


atividade 14




void main() {
  // ===== ENTRADAS =====
  double num1 = 10;
  double num2 = 0;
  String operador = '/';
  // ====================


  if (operador == '+') {
    print('Resultado: ${num1 + num2}');
  } else if (operador == '-') {
    print('Resultado: ${num1 - num2}');
  } else if (operador == '*') {
    print('Resultado: ${num1 * num2}');
  } else if (operador == '/') {
    if (num2 == 0) {
      print('Erro: divisão por zero não é permitida.');
    } else {
      print('Resultado: ${num1 / num2}');
    }
  } else {
    print('Erro: operador inválido.');
  }
}


atividade 15
void main() {
  // ===== ENTRADAS =====
  int saque = 380;
  // ====================


  if (saque <= 0 || saque % 10 != 0) {
    print('Saque não é possível: informe um valor positivo múltiplo de 10.');
  } else {
    int resto = saque;


    int notas100 = resto ~/ 100;
    resto = resto % 100;


    int notas50 = resto ~/ 50;
    resto = resto % 50;


    int notas20 = resto ~/ 20;
    resto = resto % 20;


    int notas10 = resto ~/ 10;


    print('Notas entregues:');
    print('$notas100 de 100');
    print('$notas50 de 50');
    print('$notas20 de 20');
    print('$notas10 de 10');
  }
}

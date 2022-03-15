# JuegoGrupo4

int random1()
{
  // Función que devuelve de manera aleatoria un número entero entre 0 y 1.
  int numero; 
  numero = random() % 2;
  return numero;
}

void ganador(int respuesta, int numero){
  // Procedimiento que solicita 2 números, uno es la respuesta del jugador (derecha o izquierda) y la otra es el número aleatorio de la función anterior. Compara los números y dependiendo si son iguales o no, imprime un mensaje especifico.
  if (respuesta == numero){
    printf("Muy bien, continúa.\n\n");
  }
  else {
    printf("Mala elección, HAS MUERTO.");
  }
}

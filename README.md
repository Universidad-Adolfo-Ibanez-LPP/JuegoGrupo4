# JuegoGrupo4

void puente(int intento, int lado)
{
  // Procedimiento que solicita 2 números, el número de intento del juego, y el lado elegido por el jugador (0 o 1). Se genera el puente, el cual es una matriz de caracteres. Luego mediante un ciclo anidado se imprime la posición del jugador, dependiendo de los parametros dados.
  
  char *puente[11][6] = {{"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"},
  {"[", " ", "]", "[", " ", "]"}};

  int a;
  if (lado==0){
    a = 1;
  }
  else {
    a = 4;
  }
  
  int i;
  int j;
  
  for (i = 0; i < 11; i++) {
    for (j = 0; j < 6; j++){
      puente[11-intento][a] = "O";
      printf("%s", puente[i][j]);
    }
    
    printf("\n");
  };
  printf("\n");
}

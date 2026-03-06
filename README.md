# atividade-4q
1-
#include <stdio.h>
#include <math.h>

int main() {
    float A, B, C;
    float delta, x1, x2;

    printf("Digite os valores de A, B e C: ");
    scanf("%f %f %f", &A, &B, &C);
    if (A == 0) {
        printf("Nao e uma equacao de segundo grau.\n");
      } 
      else 
	    {
        delta = (B * B) - (4 * A * C);
        if (delta < 0) {
            printf("Nao existem raizes reais.\n");
      } 
		  else 
		  {
            x1 = (-B + sqrt(delta)) / (2 * A);
            x2 = (-B - sqrt(delta)) / (2 * A);
            printf("Raiz 1 = %.2f\n", x1);
            printf("Raiz 2 = %.2f\n", x2);
      }
    }

    return 0;
}


2- 
#include <stdio.h>

int main() {
    float x, fx;
    printf("Digite o valor de x: ");
    scanf("%f", &x);
    if (2 - x == 0) {
        printf("Erro: divisao por zero nao permitida.\n");
    } 
    else 
    {
        fx = 8 / (2 - x);
        printf("f(x) = %.2f\n", fx);
    }

    return 0;
}


3- (Nao consegui resolver esse e fui corigindo com chat e outros git)
#include <stdio.h>
#include <math.h>

int main() {
    float x1, y1, z1, r1;
    float x2, y2, z2, r2;
    float distancia;
    printf("Digite o centro da esfera 1 (x y z) e o raio: ");
    scanf("%f %f %f %f", &x1, &y1, &z1, &r1);
    printf("Digite o centro da esfera 2 (x y z) e o raio: ");
    scanf("%f %f %f %f", &x2, &y2, &z2, &r2);
    distancia = sqrt(pow(x2 - x1, 2) + pow(y2 - y1, 2) + pow(z2 - z1, 2));
    if (distancia <= (r1 + r2)) {
        printf("As esferas estao colidindo ou se sobrepondo.\n");
    } 
    else 
    {
        printf("As esferas nao estao colidindo.\n");
    }

    return 0;
}


4-

#include <stdio.h>

int main() {
    float x, y;
    printf("Digite a coordenada X do drone: ");
    scanf("%f", &x);
    printf("Digite a coordenada Y do drone: ");
    scanf("%f", &y);
    if ((x >= 4 && x <= 14 && y >= 4 && y <= 10) ||
        (x >= 16 && x <= 26 && y >= 2 && y <= 11)) {
        printf("Pouso permitido em uma das regioes.\n");
    } 
    else 
    {
        printf("Pouso nao permitido.\n");
    }

    return 0;
}

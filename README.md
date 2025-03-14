# Atividade7

programa {
  funcao inicio() 
  {
    escreva("hello word: ")
  }
}

atividade 2

programa {
  funcao inicio() {
    inteiro num1, num2, soma

   leia(num1)
   leia(num2)

   soma = num1 + num2

   escreva(soma)

    
  }
}

atividade 3 

programa {
  funcao inicio() {
    inteiro num

   leia(num)

   se (num % 2 == 0)
      escreva("Par")
   senao
      escreva("Ímpar")
  }
}

atividade 4

programa {
  funcao inicio() {
    inteiro num1, num2

   leia(num1)
   leia(num2)

   se (num1 > num2)
      escreva(num1)
   senao
      escreva(num2)
    
  }
}


atividade 5

programa {
  funcao inicio() 
  {
    real n1, n2, n3, media

    escreva("Digite o primeiro número: ")
    leia(n1)
    escreva("Digite o segundo número: ")
    leia(n2)

    escreva("Digite o terceiro número: ")
    leia(n3)
    media = (n1 + n2 + n3) / 3
    escreva("A média aritmética dos números ", n1, ", ", n2, " e ", n3, " é: ", media)


  }
}

atividade 6

programa {
  funcao inicio() 
  {
    real raio, area
    const real PI = 3.14159
      escreva("Digite o raio do círculo: ")
    leia(raio)

    area = PI * (raio * raio)
     escreva("A área do círculo com raio ", raio, " é: ", area)
     


  }
}


atividade 7

programa {
  funcao inicio() 
  {
      real celsius, fahrenheit

      escreva("digite a temperatura em graus celcius: \n")
      leia(celsius)

      fahrenheit = (celsius * 9/5) + 32
      escreva("A temperatura de ", celsius, "°C equivale a ", fahrenheit, "°F.")
  }
}


atividade 8

programa {
  funcao inicio() 
  {
    inteiro n
    inteiro i
    inteiro res
    
    escreva("Informe um número para tabuada: ")
    leia(n)
    para(i=1; i<=12; i++){
      res = n*i
      escreva("\n", n , "*" , i , "=", res)
      }
    
  }
}

atividade 9

programa {
  funcao inicio() {
    inicio
   inteiro num, fatorial, i

   leia(num)

   se (num < 0) 
      escreva("Fatorial não existe para números negativos")
   senao
      fatorial = 1
      para (i=1;  i=<=30; i++){
         fatorial = fatorial * i

      escreva(fatorial)

    }
  }
}


atividade 10 

programa {
  funcao inicio() 
  {
        inteiro cont=1
        enquanto(cont<=10) {
          escreva("\n"+cont)
          cont++
          }
          escreva("contagem regressiva finalizada ")
  }
}


atividade 11

programa {
  funcao inicio() 
  {
      inteiro n, primo, resultado=1
      escreva("Determine se um numero é primo: ")
      leia(n)
      para(primo = n; primo>=1; primo --){
      resultado = resultado * primo
      escreva(n, "1 = ", resultado, "\n")
      }
      
  }
}


atividade 12

programa {
  funcao inicio() 
  {
    inteiro soma = 0, intervalo=0
    escreva("digite o intervalo para a soma.: ")
    leia(intervalo)

    para(inteiro i=1; i<=intervalo; i++){

      soma = soma + i

      }
      escreva("A soma dos numero entre 1 e "+intervalo+"="+soma)
  }
  
}


atividade 13

programa
{
	funcao inicio()
	{
		inteiro numero
		 
		escreva("Quantos elementos da sequência de Fibonacci deseja calcular? ")
		leia(numero)

		
		para (inteiro i = 1; i <= numero ; i++)
		{
			escreva(fibonacci(i), " ") 
		}

		escreva("\n")
	}

	
	funcao inteiro fibonacci(inteiro posicao)
	{		
		se (posicao == 1)
		{
			retorne 0
		}
		senao se (posicao == 2)
		{
			retorne 1
		}

		retorne fibonacci(posicao - 1) + fibonacci(posicao - 2)		
	}
}


atividade 14

programa {
  funcao inicio() 
  {
      inteiro numero, inverso, resto
      escreva("digite um numero inteiro: \n")
      leia(numero)
      inverso = 0
        enquanto(numero > 0)
      {
      resto = numero % 10
      inverso = inverso * 10 + resto
      numero = numero / 10
      }
      
      escreva(" o numero invertido é: ", inverso)
      }
  }
}

atividade 15

programa {
  funcao inicio() 
  {
      inteiro i, base, expoente, resultado=1
      escreva("digite a base: ")
      leia(base)

      escreva("digite o expoente: ")
      leia(expoente)
      resultado=1

      para(i=1; i<=expoente; i++){
        resultado = resultado * base
        }



        escreva("O resultado de ", base, " elevado a ", expoente, " é: ", resultado)
  }
}


atividade 16

programa {
  funcao inicio() 
  {
      inteiro n1, n2, resto

       escreva("Digite o primeiro número: ")
    leia(n1)
    escreva("Digite o segundo número: ")
    leia(n2)

        enquanto (n2 > 0)
        { 
        resto = n1 % n2
        n1 = n2
        n2 = resto
        }

        escreva("O MDC é: ", n1)
  }
}

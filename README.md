# Kotlin_Atividade-1📚

## 1- Construa um programa que calcule o IMC – Índice de Massa Corporal e ainda exiba aclassificação de acordo com a tabela de classificação da OMS.
## Classificação do IMC:
### Menor que 18,5 - Abaixo do peso
### Entre 18,5 e 24,9 - Peso normal
### Entre 25 e 29,9 - Sobrepeso (acima do peso desejado)
### Igual ou acima de 30 – Obesidade
---
# Resposta🎯:

```Kotlin

```
import kotlin.math.pow

fun main() {

    print("Digite seu peso: ")
    val peso = readLine()!!.toDouble()

    print("Digite sua altura: ")
    val altura = readLine()!!.toDouble()

    val imc = peso / altura.pow(2)

    val classificacao = when {
        imc < 18.5 -> "Abaixo do peso"
        imc < 25 -> "Peso normal"
        imc < 30 -> "Sobrepeso"
        else -> "Obesidade"
    }

    println("IMC: $imc")
    println("Classificação: $classificacao")

}


Go Do zero ao avançado

Características

Inicialmente concebido para resolver problemas de concorrência, mas com desejo de manter a simplicidade no desenvolvimento.

Não precisa de máquina virtual. A compilação já é feita em uma versão executável, e dedicada para cada sistema operacional.
Não existe um serviço centralizado de compilação de pacotes
As interfaces são implícitas (Não precisa de um public class struct implements)

Estruturas de arquivos

Em go toda execução de programa começa pela função main dentro de um package main, sem essa função o programa vai gerar erro de compilação.

package main

import "fmt"

func main() {
	fmt.Println("Hello World")
}


Variáveis

Utiliza a palavra reservada “var” para criação de variáveis. É necessário atribuir tipo e um valor a essa variável caso isso não ocorra haverá um erro de compilação devido a atenção que a linguagem da a performance e ao uso de memória, se uma variável não é utilizada ela deve ser excluída. 

Tipos de dados

Em golang os tipos de dados são estáticos ou seja o tipo não pode ser modificado em tempo de execução.

tipos que começam com u são do tipo não assinados ou seja só permite valores positivos
 uint8 8-bit unsigned int 




Existe uma forma de criação e atribuição simultaneamente utilizando o operador “:=”.


package main

import "fmt"

func main() {
	message := "Hello World"
	fmt.Println(message)
}


Conversão 

Para converter int e float entre eles é possível utilizar apenas parênteses


package main

import "fmt"

func main() {

	var (
		numeroF float32
		numeroI uint8
	)
	numeroF = 99.5
	numeroI = uint8(numeroF)

	fmt.Println(numeroI)
}
```


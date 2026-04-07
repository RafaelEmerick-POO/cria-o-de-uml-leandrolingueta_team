# Exemplo de Documentação UML

## Introdução
A UML (Unified Modeling Language) é uma linguagem de modelagem utilizada para visualizar, especificar, construir e documentar sistemas de software.  
Ela permite representar estruturas como classes, objetos e seus relacionamentos.

## Diagrama de Classes
Abaixo temos um exemplo simples de diagrama de classes usando Mermaid:

```mermaid
classDiagram

Equipamento <|-- sensor

class Equipamento {
    -string tag
    -string descricao
    -bool ativo
    +string tagEquipamento
    +string descricaoEquipamento
    +bool ativoInicial
    +void ligar()
    +void desligar()
    +string getTag()
    +bool estaAtivo()
    +virtual void exibirResumo()
    +virtual Equipamento()
}

class sensor{
    -double valorAtual
    +string tagSensor
    +string descricaoSensor
    +bool ativoInicial
    +double valorInicial
    +void atualizarLeitura()
    +double getValorAtual()
    +void exibirResumo()
}
```


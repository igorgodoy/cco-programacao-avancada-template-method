# Programação Avançada

Atividade padrão de projeto - **Template Method**.

## Conteúdos

1. [Classificação](https://github.com/igorgodoy/cco-programacao-avancada-template-method#classifica%C3%A7%C3%A3o)
2. [Intenção](https://github.com/igorgodoy/cco-programacao-avancada-template-method#inten%C3%A7%C3%A3o)
3. [Motivação](https://github.com/igorgodoy/cco-programacao-avancada-template-method#motiva%C3%A7%C3%A3o)
4. [Aplicação](https://github.com/igorgodoy/cco-programacao-avancada-template-method#aplica%C3%A7%C3%A3o)
5. [Estrutura](https://github.com/igorgodoy/cco-programacao-avancada-template-method#estrutura)
6. [Implementação](https://github.com/igorgodoy/cco-programacao-avancada-template-method#implementa%C3%A7%C3%A3o)

## Template Method

### Classificação

- O **Template Method** é um padrão de projeto que, literalmente, define o *Template* de um algoritmo na superclasse e permite que suas subclasses sobrescrevam métodos específicos do algoritmo, ou mesmo criem novos, sem modificar sua estrutura.

### Intenção

- Abstrair o esqueleto de um processo, permitindo particularidades de alguns passos para seus subprocessos.

### Motivação

- Este padrão de projeto é fundamental e pode ser encontrado em quase todas as classes abstratas.

### Aplicação

- Um software que extrai dados de diferentes tipos de arquivos pode ser um ótimo exemplo. Neste cenários temos uma superclasse *FileExtract* contendo alguns métodos comuns à todos os tipos de arquivos como *openFile* e *closeFile*, e desta superclasse podemos derivar as subclasses *CSVFileExtract* e *TXTFileExtract*, onde estas subclasses terão seus próprios métodos *extractData*, com sua tratativas particulares.

### Estrutura

- A estrutura de um **Template Method** consiste basicamente na criação de uma superclasse contendo parte dos métodos, imutáveis e comuns à todas suas subclasses variantes, e a criação destas subclasses contendo a implementação dos demais métodos específicos unicamente à ela. Este [diagrama](https://refactoring.guru/images/patterns/diagrams/template-method/structure.png) representa uma classe abstrata desenhada a partir deste padrão de projeto.

### Implementação

- [Example](https://github.com/igorgodoy/cco-programacao-avancada-template-method/tree/master/example).

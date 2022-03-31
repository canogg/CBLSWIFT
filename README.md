# Como cobrar por projetos de arquitetura 👷🏻‍♀️

Esse script foi pensado para otimizar a cobrança de projetos de arquitetura, pois muitas questões devem ser consideradas na hora de precificar o trabalho de um arquiteto.

> Status do Projeto: :heavy_check_mark: :warning: (concluido, em desenvolvimento)

### Tópicos 

:small_blue_diamond: [Motivos](#motivos)

:small_blue_diamond: [Entendendo o Código](#entendendo-o-código)

# Motivo
Considerei minha experiência prévia e a dificuldade que tive durante meus anos de escritório, muitas vezes o valor cobrado não era o correto. Outro motivo para a criação desse script foi que percebi esse tipo de dificuldade em vários colegas de trabalho.
# Entendendo o código
  Primeiro é importante saber que um projeto de arquitetura tem várias etapas: estudo preliminar, anteprojeto, projeto executivo. No estudo preliminar é feito o levantamento, que são as medições necessárias para iniciar o projeto, isso é passado para o autocad e inicia o programa de necessidades logo depois são feitas as plantas gerais do anteprojeto, tendo a aprovação do cliente passamos para a modelagem 3D, e renderização, após essa etapa aprovada segue para o projeto executivo onde são feitas as plantas que serão levadas para a obra, podendo ter ou não projeto de marcenaria. Quando a obra é iniciada o arquiteto pode fazer algumas visitas técnicas na obra.
  
  ## 🚀 Instalando

Para instalar o Setterfolder siga estas etapas:

macOS (Somente):

Primeiramente, faça clone do projeto pelo o comando:
```
git clone https://github.com/JoanWilson/Setterfolder.git
```

# Explicação do código:
- Primeiro foi levado em consideração o tipo de projeto utilizando switch case
Se for arquitetônico o programa da as operações de ambientes residênciais de projetos arquitetonicos 
Se for interiores o programa da as opções de ambientes para este módulo
Se for comercial o programa da as opções de ambientes para este módulo
- Você digita os ambientes que serão projetados e cada ambiente terá um valor adicionado a função final dependendo da dificuldade e tempo de projeta-lo, foi utilizado for e if else para adicionar o valor na função final
- Depois foi levado em consideração se terá ou não levantamento com if e else, se tiver o programa perguntará a distância até o local para calcular quanto você gastará de gasolina e adicionar na função final juntamente com o valor do preço do levantamento
- Também foi levado em consideração o tempo que o arquiteto passará em cada programa, coloquei os 3 principais que utilizo, Autocad, Sketchup, Lumion e isso foi multiplicado pelo valor da hora e adicionado a função final
- Outro aspecto levado em consideração foi o fato de ter marcenaria ou não no projeto utilizando if e else será adicionado um valor final a função ou não
- Por último se terá ou não visita técnica na obra utilizando if e else
- Juntei tudo numa função final para calcular o valor que deve ser cobrado para o cliente.

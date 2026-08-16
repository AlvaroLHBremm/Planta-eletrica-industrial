# Planta eletrica industrial com quadro de cargas
Projeto acadêmico desenvolvimento utilizando FreeCAD durante a disciplina `maquina e acionamentos` de uma planta elétrica industrial
e comercial completa, incluindo quadro de cargas, dimensionamento de circuitos e dispositivos de proteção, com foco em aplicações industriais.

<p align="center"> <img src="figs/planta_completa.png" alt="diagrama" width="100%"></p>
<p align="center"><b>planta elétrica</b></p>

# Metodologia

Durante a criação da planta foi dividido cada comodo de modo a aplicar as normas de iluminação proporcional a area e as normas de tomadas de uso geral proporcional ao perimetro do comodo. Em contraste, as tomadas de uso expessifico foram adicionados em comodos grandes para suportar ar-condicionaos e em banheiros para suportar chuveiros, suas potencias foram estipuladas de acorda com a média de potencia dos ar-condicionados e chuveiros do mercado.

Calculo de BTU: 600 BTU por m/2.

BTU para watts: BTu * 0,293

<p align="center"> <img src="figs/planta.png" alt="diagrama" width="100%"></p>
<p align="center">Planta</p>

Devido a extensão deste projeto em conjunto de demais projetos da mesma disciplina, o professor regente autorizou a simplificação de certos cálculos. Para a corrente de dimensionamento foi adicionado um fator de margem de segurança de 25% para substituir fatores de agrupamento e de temperatura em relação a espessura da bitola do ramal.

## Fatores de potencia

Levando em conta que edificios comerciais possuem uma rotação de pessoas significativa, pode-se estiupular os calculos de correntes não pelo maximo disponivel, mas sim pela média de utilização. Ai entra os fatores de potencia com o intuito de diminuir custos associando habitos as necessidades de energia da maneira mais eficiente. Para este projeto fou estipulato fatores de utilização de 70% para os circuitos de iluminação, 80% Para os circuitos das tomadas de uso geral e 100% para as tomadas de uso exclusivo, pois devido a sua alta potencia, mesmo com baixo uso, não se deve estipular para baixo sua corrente e condutor.


| Fator  de potencia | valor |
| :---: | :--- |
| `Iluminação` | 0,70 |
| `TUG` | 0,70 |
| `TUE` | 0,70 |

### Fatores de potencia industrial
Para mas maquininhas

| Fator  de potencia | valor |
| :---: | :--- |
| `utilização` | 0,70 |
| `Simultaneadade` | 0,85 |

### Fatores de demanda
| Fator  de potencia | valor |
| :---: | :--- |
| `utilização` | 0,70 |
| `Simultaneadade` | 0,85 |

## Divisão de potencia

Devido a alimentação trifasica do edificio, é importante balancear a carga de cada fase uniformemente, pois com a diminuição do condutor devido ao efeito triasico , pode-se atribuir muita carga a uma fase, ultrapassando a corrente estiulada dos condutores. Por isso na tabela abaixo, na coluna `fase`, cada circuito é atribuida a uma fase do modo mais balanceado possivel para o projeto.


| Fase | potencia |
| :---: | :--- |
| `R` | 11560 W |
| `S` | 13180 W |
| `T` | 12000 W |

<p align="center"> <img src="figs/parametros.png" alt="diagrama" width="100%"></p>
<p align="center">Planta</p>

A planta do projeto se trada de um edificio hipetético, sendo igual para todos os alunos, diferindo-se levemente a depender de como o aluno reproduziu o desenho em softwares como AutoCAD ou FreeCAD. O layout do projeto se trada de um edificio hipetético


Memorial técnico](https://github.com/AlvaroLHBremm/Planta-eletrica-industrial/blob/main/docs/memorial.pdf)




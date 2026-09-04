# Segmentação de Lâminas Petrográficas

#### Repositório para orientação e avanços na segmentação de objetos em lâminas petrográficas

🔗GitHub: `https://github.com/LCCMat-UnB/segmentacao-laminas/`

### Instruções

​	Em breve

------

| Nome    | Nível      | Equipe | Observação |
| ------- | ---------- | ------ | ---------- |
| Luiz    | Professor  |        |            |
| Tromer  | Professor  |        |            |
| Carlos  | PosDoc     |        |            |
| Hugo    | Doutorando |        |            |
| Israel  | Doutorando |        |            |
| Ana     | Mestranda  |        |            |
| Érick   | Mestrando  |        |            |
| Davi    | Graduando  |        |            |
| Dimitry | Graduando  |        |            |
| Larrisa | Graduando  |        |            |
| William | Graduando  |        |            |



------

### Tasks iniciais

- [ ]  Implementação das métricas petrofísicas no pacote `rockface` (@oi-silva).
- [ ]  Dados morfológicos de poro para correlacionar lâminas (@HugoXR).



------

### Fluxos de trabalho

```
Fluxo 1: Equipe A | Fluxo 2: Equipe B | Fluxos 3 e 4: N/A
```

#### 1. Segmentação baseada em IA de poros

##### Objetivos gerais

Utilização de imagens pré-segmentadas pelo pacote `rockface` para implementação de um modelo de Machine Learning de segmentação de poros em secções finas.

##### Objetivos específicos (tasks)

1. Prospecção de modelos para o dataset

- [ ]  Buscar na literatura de modelos aplicados/testados para segmentação de imagens (que possam ser transladados para o contexto desta pesquisa);
- [ ]  Estudar o desempenho de diferentes modelos (orientados pela literatura consultada) de segmentação via inteligência artificial;
- [ ]  Determinar melhores modelos (incluindo parâmetros gerais da arquitetura e do dataset) candidatos para aplicação em escala no projeto;
- [ ]  Viabilizar a produção de um paper.

2. Aplicar e avaliar a arquitetura candidata

- [ ]  Preparar o dataset completo (disponível) para segmentação dos poros via imagem pré-segmentadas;
- [ ]  Aplicar modelo candidato;
- [ ]  Avaliar quantitativamente, via métricas tradicionais e petrofísicas, e qualitativamente, com time de especialistas, a qualidade das máscaras segmentadas.

3. Preparar do pipeline para segmentação de grãos.

#### 2. Prospecção de metodologias para segmentação de grãos

##### Objetivos gerais

Pré-segmentar grãos em lâminas petrográficas e retreinar modelo selecionado pela equipe de poros.

##### Objetivos específicos (tasks)

1. Escolha da metodologia para anotação de grãos

- [ ]  Buscar na literatura para determinar formas de pré-segmentar grãos (como, por exemplo, modelos de IA já treinados, buscar pelo dinov3) para preparação do dataset de treino [do modelo que estamos propondo];
- [ ]  Entender como as imagens polarizadas podem melhorar a segmentação (a imagem polarizada é também utilizada para distinguir corpos de grãos);
- [ ]  Iniciar testes de pré-segmentação de grãos nas lâminas petrográficas;
- [ ]  Avaliar quantitativamente, via métricas tradicionais e petrofísicas, e qualitativamente, com time de especialistas, a qualidade das máscaras segmentadas;

2. Segmentação de poros e grãos

- [ ]  Preparar o dataset completo (disponível) para segmentação dos poros via imagem pré-segmentadas;
- [ ]  Fine tunning do modelo selecionado e treinado pela equipe dos poros (task 1.2);
- [ ]  Avaliar quantitativamente, via métricas tradicionais e petrofísicas, e qualitativamente, com time de especialistas, a qualidade das máscaras segmentadas; é importante medir a qualidade das máscaras de poros e grãos neste passo;

#### 3. Classificação dos poros

##### Objetivos gerais

Buscar metodologias para viabilizar a classificação de poros, com base na teoria geológica (Textural e Morfológica).

#### 4. Classificação dos grãos

##### Objetivos gerais

Buscar metodologias para viabilizar a classificação de grãos, com base na teoria geológica (Granulometria, Grau de Seleção, Morfologia e Arredondamento).

------


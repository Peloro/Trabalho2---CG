# Computação Gráfica - Projetos T02 e T03

Este repositório contém os trabalhos desenvolvidos para a disciplina de Computação Gráfica utilizando OpenGL moderno.

Os projetos estão organizados em diretórios separados:

- **T02/** → Projeto 2: Construção de cenário 3D com texturas e exploração por câmera.
- **T03/** → Projeto 3: Extensão do Projeto 2 com sistema de iluminação ambiente, difusa e especular.

## Estrutura do Repositório

```
.
├── T02/
│   └── Projeto 2
├── T03/
│   └── Projeto 3
└── README.md
```

---

# T02 — Cenário 3D Texturizado

O Projeto 2 tem como objetivo a construção de um cenário 3D composto por ambientes interno e externo, utilizando modelos importados no formato Wavefront (.obj) e aplicação de texturas.

## Funcionalidades

- Importação de modelos 3D (.obj)
- Aplicação de texturas
- Ambiente interno e externo
- Controle de câmera para exploração da cena
- Skybox para representação do céu
- Visualização de malha poligonal (wireframe)
- Transformações geométricas:
  - Translação
  - Rotação
  - Escala

## Tecnologias Utilizadas

- OpenGL (Pipeline Moderno)
- GLFW
- GLM
- TinyOBJLoader
- stb_image

## Objetivos Acadêmicos

- Manipulação de matrizes Model, View e Projection
- Renderização de modelos texturizados
- Navegação em ambientes 3D
- Organização de cenas complexas

---

# T03 — Sistema de Iluminação

O Projeto 3 é uma evolução direta do Projeto 2. A cena foi expandida para incorporar modelos de iluminação utilizando componentes ambiente, difusa e especular.

## Funcionalidades Adicionadas

### Iluminação Ambiente

- Intensidade ajustável por teclado
- Pode ser ligada ou desligada independentemente

### Iluminação Difusa

- Ajuste em tempo real da reflexão difusa
- Parâmetros individuais para cada objeto

### Iluminação Especular

- Ajuste em tempo real da reflexão especular
- Configuração individual para cada objeto

### Fontes de Luz

#### Ambiente Externo

- Fonte de luz associada a um objeto em movimento
- Afeta exclusivamente objetos externos

#### Ambiente Interno

- Duas fontes de luz independentes
- Cores diferentes
- Afetam exclusivamente objetos internos

### Controles

- Ligar/desligar cada luz individualmente
- Incrementar/decrementar luz ambiente
- Incrementar/decrementar reflexão difusa
- Incrementar/decrementar reflexão especular

## Conceitos Aplicados

- Modelo de iluminação de Phong
- Cálculo de normais
- Shaders GLSL
- Múltiplas fontes de luz
- Separação de grupos de iluminação
- Atualização dinâmica de uniform variables

---


# Observações

- O diretório **T03** reutiliza e expande a base desenvolvida em **T02**.
- Ambos os projetos utilizam exclusivamente recursos do **OpenGL Moderno**, sem o uso de funções depreciadas do pipeline legado.
- Os modelos e texturas utilizados pertencem aos seus respectivos autores e foram empregados apenas para fins acadêmicos.

---

## Disciplina

**Computação Gráfica**

Instituto de Ciências Matemáticas e de Computação (ICMC-USP)

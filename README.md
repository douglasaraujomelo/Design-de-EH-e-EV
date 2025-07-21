# Design-de-EH-e-EV
Projeto de análise das empenagens traseiras no XFLR5
# Empenagens UAV – Estudo no XFLR5

Este repositório documenta o projeto, modelagem e análise das empenagens horizontais (EH) e verticais (EV) de uma aeronave não tripulada (UAV), utilizando o software XFLR5 v6.61.

---

## ✈️ Descrição do Projeto

O objetivo é projetar as superfícies de cauda (EH e EV), considerando:
- Equilíbrio estático (`Cm0`)
- Estabilidade longitudinal e direcional
- Estol diferenciado entre asa e empenagem
- Posicionamento adequado dos servomotores

---

## 📐 Geometria e Parâmetros Utilizados

### 📌 Empenagem Horizontal (EH)
- **Perfil**: S1223
- **Braço (alavanca)**: `0,600 m`
- **Cm0** (momento de arfagem): `+0,02`
- **Volume de cauda horizontal (Vh)**: `0,41`
- **Estol posterior ao da asa**: ≥ `+5°`

### 📌 Empenagem Vertical (EV)
- **Perfil**: NACA0015
- **Braço (alavanca)**: `0,650 m`
- **Área estimada**: `0,03 m²`

---

## ⚖️ Massa e Centro de Gravidade (CG)

### 📊 Densidade do material:
- `0,35 g/mm³` = `350 kg/m³`

### 📦 Massas alocadas:
| Componente | Massa (kg) | Posição x (m) | Descrição       |
|------------|------------|----------------|-----------------|
| EH         | 0,386      | 0,600          | Horizontal Tail |
| EV         | 0,155      | 0,650          | Vertical Tail   |
| Servo EH   | 0,050      | 0,600          | Servo Elevador  |
| Servo EV   | 0,050      | 0,650          | Servo Leme      |

### 📍Centro de Gravidade Calculado:
- **Total mass**: `0,641 kg`
- **X_CoG**: `~0,624 m` (aproximado)

---

## ⚙️ Servomotores

Os servos foram posicionados **próximos da raiz das empenagens**, com o objetivo de:

- Reduzir o momento de inércia
- Manter o centro de gravidade ideal
- Facilitar a manutenção e instalação

📌 **Posições definidas:**
- Servo EH: `x = 0,600 m`
- Servo EV: `x = 0,650 m`
- **Massa de cada servo**: `0,050 kg`

---

## 🧪 Software Utilizado

- [XFLR5 v6.61](http://www.xflr5.com/xflr5.htm)
- Análise 3D com método de painéis (Vortex Lattice Method - VLM)

---

## 📁 Organização futura do repositório

---

## ✍️ Autor

Projeto por: **[Douglas Melo e Júlia Vanderlay]**  
Instituição: [Universidade Federal de Pernambuco - Mandacaru Aerodesign-Treinee]

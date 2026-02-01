# 🐠 Calculadora de Consumo de Energia para Aquário

Uma aplicação web simples e intuitiva para calcular o consumo de energia elétrica dos equipamentos do seu aquário, desenvolvida para ajudar aquaristas a estimar seus gastos mensais com eletricidade.

![Screenshot da Calculadora](https://img.shields.io/badge/Status-Pronto-success)
![Versão](https://img.shields.io/badge/Vers%C3%A3o-1.0-blue)

## 📋 Sobre o Projeto

Esta calculadora permite que você:
- Adicione múltiplos equipamentos do aquário
- Configure potência (em Watts) e tempo de uso diário
- Defina quantidades de equipamentos idênticos
- Selecione seu estado para preenchimento automático da tarifa
- Visualize consumo e custo diário, mensal e anual
- Obtenha um resumo detalhado por equipamento

## ✨ Funcionalidades

### 🔌 Gerenciamento de Equipamentos
- Lista pré-definida de equipamentos comuns:
  - Aquecedor
  - Bomba do Filtro
  - Luminária
  - Chiller
  - Filtro UV
  - Skimmer
  - Ventoinha Cooler
  - Wave Maker
  - E mais...
- Possibilidade de adicionar equipamentos personalizados
- Campo de quantidade para equipamentos duplicados

### ⚡ Cálculo de Consumo
- Consumo em kWh (diário, mensal e anual)
- Custo em R$ (diário, mensal e anual)
- Seleção de estado para tarifa automática
- Edição manual de tarifa disponível

### 📊 Visualização
- Resumo detalhado de cada equipamento
- Interface limpa e moderna
- Design responsivo para mobile
- Tema aquático com gradientes

## 🚀 Como Usar

1. **Selecione seu estado** para preencher automaticamente a tarifa de energia
2. **Clique em "+ Adicionar Equipamento"**
3. **Preencha os dados:**
   - Nome do equipamento (use o autocomplete ou digite)
   - Potência em Watts
   - Quantidade de equipamentos
   - Horas de funcionamento por dia
4. **Clique em "Adicionar"**
5. **Visualize os resultados** no card de consumo total

## 🛠️ Tecnologias Utilizadas

- **HTML5** - Estrutura
- **CSS3** - Estilização e animações
- **JavaScript Vanilla** - Lógica e interatividade
- **Google Fonts** - Tipografia (Outfit e JetBrains Mono)

## 📦 Estrutura do Projeto

```
calculadora-aquario/
│
├── calculadora-aquario.html    # Arquivo principal (standalone)
└── README.md                   # Este arquivo
```

## 🎨 Design

- **Paleta de cores aquática** com tons de azul e turquesa
- **Tipografia moderna** com Outfit para textos e JetBrains Mono para números
- **Animações suaves** para melhor experiência do usuário
- **Layout responsivo** que se adapta a diferentes tamanhos de tela

## ⚙️ Personalização

### Atualizar Tarifas por Estado

No arquivo `calculadora-aquario.html`, localize o objeto `tarifasPorEstado` e atualize os valores:

```javascript
const tarifasPorEstado = {
    'AC': 0.70,  // Atualize com valor real
    'AL': 0.71,  // Atualize com valor real
    // ... demais estados
};
```

### Adicionar Novos Equipamentos Padrão

Localize o array `equipamentosPadrao` e adicione novos itens em ordem alfabética:

```javascript
const equipamentosPadrao = [
    'Aquecedor',
    'Seu Novo Equipamento',
    // ... demais equipamentos
];
```

## 📱 Compatibilidade

- ✅ Chrome/Edge (Chromium)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
- ✅ Navegadores móveis (iOS/Android)

## ⚠️ Aviso Legal

Os valores de tarifa e cálculos apresentados são apenas para simulação e estimativa. Não possuem validade legal. Para valores exatos, consulte sua concessionária de energia elétrica.

## 👨‍💻 Autor

**João Paulo Pompei**

Desenvolvido com auxílio de Claude AI (Anthropic)

## 📄 Licença

Este projeto é de código aberto e está disponível para uso pessoal e educacional.

---

## 🤝 Contribuições

Sugestões e melhorias são bem-vindas! Sinta-se à vontade para:
- Reportar bugs
- Sugerir novas funcionalidades
- Melhorar a documentação

## 📞 Contato

Para dúvidas ou sugestões, abra uma issue no repositório.

---

**Desenvolvido com 💙 para a comunidade de aquarismo**

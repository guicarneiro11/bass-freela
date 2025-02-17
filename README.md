# Bass Emulator Android App

## Sobre o Projeto
Um emulador de contra-baixo desenvolvido para Android, inspirado no [Real Bass](https://play.google.com/store/apps/details?id=br.com.rodrigokolb.realbass). O projeto é uma implementação que combina interatividade precisa, feedback visual realista e controle de áudio.

https://github.com/user-attachments/assets/5ce5d6b4-181f-4055-b739-5313f6c0b4eb

## Funcionalidades Principais
- 🎸 Interface completa do braço do baixo com 22 trastes
- 🎵 4 cordas com sons distintos (G, D, A, E) e espessuras diferentes
- 🎯 Sistema de feedback visual com:
  - Animações personalizadas de vibração das cordas
  - Efeitos de toque com cores específicas para cada corda
  - Indicadores visuais de posicionamento
- 🔄 Sistema de navegação pelo braço com:
  - Controle de posição via palheta deslizante
  - Ajuste dinâmico da escala dos trastes
  - Transições suaves entre posições
- 🎚️ Controle de execução:
  - Botão de Sustain para controle da duração das notas
  - Função Stop All para interrupção imediata
  - Resposta tátil ao toque nas cordas

## Tecnologias Utilizadas
- **Linguagem**: Kotlin + XML
- **Custom Views**: 
  - Implementação de views personalizadas
  - Sistema próprio de renderização e animação
  - Gerenciamento de estados visuais
- **Arquitetura**: 
  - MVVM + Clean Architecture
  - Gerenciamento de estados com LiveData
  - Coroutines para operações assíncronas
- **Injeção de Dependência**: Koin
- **Audio**: Android SoundPool com gerenciamento de estados
- **Animações**: Sistema customizado de animações com ValueAnimator

## Destaques Técnicos
- Sistema complexo de Custom Views Android com:
  - Cálculos precisos de posicionamento e escala
  - Gerenciamento de touch events multitoque
  - Sistema próprio de feedback visual
- Sistema de áudio otimizado com:
  - Controle granular de reprodução
  - Gerenciamento de estados de sustain
  - Transições suaves entre notas
- Animações sofisticadas com:
  - Sistema próprio de vibração de cordas
  - Efeitos visuais responsivos
  - Controle preciso de estados de animação
- Arquitetura robusta com:
  - Gerenciamento eficiente de estados
  - Separação clara de responsabilidades
  - Alta testabilidade e manutenibilidade

## Desafios e Soluções

1. **Precisão no Posicionamento e Escala**
   - Implementação de sistema de cálculo de trastes
   - Ajuste automático de escala baseado na posição
   - Mapeamento preciso de toques para notas

2. **Gerenciamento de Estados de Áudio e Animação**
   - Sistema de estados para sustain
   - Coordenação entre feedback visual e áudio
   - Controle granular de animações das cordas

3. **Performance e Responsividade**
   - Otimização de renderização e animações
   - Sistema de gerenciamento de recursos
   - Minimização de alocações de objetos

4. **Arquitetura e Manutenibilidade**
   - Implementação de Clean Architecture
   - Sistema modular e extensível
   - Componentes reutilizáveis e testáveis

## Arquitetura

```plaintext
com.guicarneirodev.bassproject/
├── core/
│   └── di/
├── data/
│   ├── repository/
│   └── datasource/
├── domain/
│   ├── model/
│   ├── repository/
│   └── usecase/
├── presentation/
│   ├── bass/
│   └── model/
└── ui/
    ├── components/
    ├── effects/
    └── animations/
```

## Licença
Este projeto é privado e foi desenvolvido como parte de um trabalho freelance. O código fonte não está disponível publicamente.

## Autor
[Guilhere Carneiro] - [LinkedIn](https://www.linkedin.com/in/guicarneiro1/)
- Desenvolvedor Android

---

*Nota: Este projeto foi desenvolvido como parte de um trabalho freelance e demonstra capacidade técnica em desenvolvimento Android nativo com foco em interfaces customizadas e interativas.*

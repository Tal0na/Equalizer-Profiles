# Perfis de Equalização

[![en](https://img.shields.io/badge/lang-en-red.svg)](/README/README.md)
[![pt-BR](https://img.shields.io/badge/lang-pt--BR-green.svg)](/README/README.pt-BR.md)
[![ru](https://img.shields.io/badge/lang-ru-yellow.svg)](/README/README.ru.md)
[![uk-UA](https://img.shields.io/badge/lang-uk--UA-blue.svg)](/README/README.uk-UA.md)

## Introdução

Este repositório contém **perfis de equalização personalizados** desenvolvidos para melhorar a qualidade de áudio em sistemas **Windows e Linux**.  
Os perfis são voltados para música, jogos, filmes e uso multimídia em geral, podendo ser adaptados a diferentes dispositivos de áudio e preferências pessoais.

---

## Plataformas e Aplicações Suportadas

### Windows
- **Equalizer APO**
- **Peace Equalizer** (interface gráfica para o Equalizer APO)

### Linux
- **EasyEffects** (PipeWire – recomendado)
- **PulseEffects** (PulseAudio – legado)
- **Filtros de equalização nativos do PipeWire**

> ⚠️ A maioria das distribuições Linux modernas (Fedora, Arch, Ubuntu 22.10+) utiliza **PipeWire** por padrão.  
> Nesse caso, o **EasyEffects** é a solução recomendada.

---

## Requisitos

### Windows
- **Equalizer APO**  
  https://sourceforge.net/projects/equalizerapo/
- **Peace Equalizer**  
  https://sourceforge.net/projects/peace-equalizer-apo-extension/

### Linux
- **EasyEffects**
  - Flatpak (recomendado):
    ```bash
    flatpak install flathub com.github.wwmm.easyeffects
    ```
  - Ou instalação via gerenciador de pacotes da sua distribuição
- **PipeWire** (normalmente já instalado)

---

## Categorias

Os perfis de equalização são organizados por **tipo de dispositivo de áudio**:

- **Earphones**  
  Dispositivos intra-auriculares como IEMs e earbuds (com fio ou sem fio).

- **Headphones**  
  Fones over-ear e on-ear para música, monitoramento e uso geral.

- **Headsets (Gamer)**  
  Headsets gamer com microfone integrado, otimizados para jogos, chat por voz e multimídia.

- **Speakers**  
  Caixas de som de mesa, caixas bookshelf e sistemas de som tradicionais.

- **Soundbars**  
  Soundbars utilizadas com TVs, monitores ou setups de mesa.

Essa estrutura garante consistência entre  
**Windows (Peace / Equalizer APO)** e **Linux (EasyEffects / PipeWire / PulseEffects)**.

---

## Como Aplicar os Perfis

### Windows (Peace Equalizer)

1. Abra o **Peace Equalizer**.
2. Configure as bandas de frequência e filtros conforme o perfil desejado.
3. Clique em **Save settings** e dê um nome ao perfil  
   Exemplo: `MyEQConfig`.
4. Para carregar um perfil:
   - Abra o Peace Equalizer
   - Vá em **Presets**
   - Selecione `MyEQConfig`

---

### Linux (EasyEffects)

1. Abra o **EasyEffects**.
2. Ative o efeito **Equalizer**.
3. Configure as bandas de frequência manualmente ou importe um preset.
4. Clique em **Presets → Save Preset**.
5. (Opcional) Atribua o preset para:
   - Saída de áudio do sistema
   - Aplicações específicas

> O EasyEffects oferece suporte a **perfis por aplicativo**, recurso que não está disponível no Equalizer APO.

---

## Notas de Compatibilidade dos Perfis

- As bandas de frequência e valores de ganho são **totalmente transferíveis** entre:
  - Peace Equalizer ↔ EasyEffects
- Alguns nomes de filtros podem variar conforme a aplicação:
  - **Preamp** → **Input Gain**
  - **Peak Filter** → **Bell Filter**
- Sempre ajuste o **preamp/input gain** para evitar clipping ou distorções.

---

## Considerações Finais

Estes perfis são baseados em **preferências pessoais** e podem não ser ideais para:
- Todo tipo de headset, fone ou caixa de som
- Todos os gêneros musicais ou cenários de uso

Sinta-se à vontade para ajustar:
- Níveis de ganho
- Valores de Q
- Volume do preamp

Se você melhorar ou adaptar um perfil para um dispositivo específico, considere compartilhá-lo com a comunidade.

---

## Referências

- Documentação do Equalizer APO  
  https://sourceforge.net/p/equalizerapo/wiki/Documentation/
- Guia do Peace Equalizer  
  https://sourceforge.net/p/peace-equalizer-apo-extension/wiki/Documentation/
- Documentação do EasyEffects  
  https://github.com/wwmm/easyeffects

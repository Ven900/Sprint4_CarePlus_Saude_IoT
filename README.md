# 🏥 CarePlus Saúde

## Sistema Inteligente de Monitoramento de Pacientes com IoT

Projeto desenvolvido para a **Sprint 3 da disciplina Edge Computing & Computer Systems**, com o objetivo de aplicar conceitos de Internet das Coisas (IoT), Edge Computing e monitoramento de dados em tempo real.

A solução utiliza um ESP32 conectado a sensores para simular o monitoramento de sinais vitais, permitindo a coleta, processamento e transmissão de informações para plataformas de visualização e análise, contribuindo para o acompanhamento remoto de pacientes.

---

## 🎯 Objetivo do Projeto

Desenvolver um sistema inteligente capaz de monitorar indicadores de saúde de pacientes em tempo real utilizando dispositivos IoT.

O projeto busca demonstrar como tecnologias embarcadas podem auxiliar no acompanhamento remoto de pacientes, contribuindo para processos de triagem, monitoramento e apoio à tomada de decisão.

---

## 🔧 Componentes Utilizados

### Hardware

* ESP32 DevKit V1
* Sensor DHT22
* Potenciômetro para simulação de BPM
* Potenciômetro para simulação de SpO₂

### Software

* Wokwi Simulator
* Arduino IDE
* MQTT
* Node-RED
* GitHub

---

## ⚙️ Funcionalidades

✅ Monitoramento de temperatura corporal

✅ Simulação de frequência cardíaca (BPM)

✅ Simulação de saturação de oxigênio (SpO₂)

✅ Classificação automática do estado do paciente

✅ Comunicação de dados utilizando MQTT

✅ Dashboard para visualização em tempo real

✅ Histórico para acompanhamento das leituras

---

## 🏗️ Arquitetura da Solução

Sensores → ESP32 → Wi-Fi → MQTT Broker → Node-RED → Dashboard → Histórico de Dados

---

## 🚨 Regras de Monitoramento

| Indicador   | Condição de Alerta |
| ----------- | ------------------ |
| Temperatura | Acima de 38°C      |
| BPM         | Acima de 100 bpm   |
| SpO₂        | Abaixo de 95%      |

Quando alguma condição crítica é identificada, o sistema classifica o paciente como:

**ATENÇÃO**

Caso contrário:

**NORMAL**

---

## 📊 Exemplo de Dados Transmitidos

```json
{
  "temperatura": 36.5,
  "bpm": 78,
  "spo2": 98,
  "status": "NORMAL"
}
```

---

## 💻 Tecnologias Aplicadas

* Internet das Coisas (IoT)
* Edge Computing
* Sistemas Embarcados
* MQTT
* Node-RED
* ESP32
* GitHub

---

## 📁 Estrutura do Projeto

```text
Sprint3-CarePlus-Saude-IoT
│
├── README.md
├── sketch.ino
├── diagram.json
├── libraries.txt
│
├── docs
│   ├── Relatorio_Sprint3.pdf
│   ├── Arquitetura.pdf
│   └── Manual_Operacao.pdf
│
├── imagens
│   ├── circuito_wokwi.png
│   ├── monitor_serial.png
│   ├── dashboard_nodered.png
│   └── arquitetura_sistema.png
│
└── video
    └── link_youtube.txt
```

## 🔗 Links do Projeto

### GitHub

Repositório oficial do projeto:

* GitHub: [https://github.com/SEU-USUARIO/Sprint3-CarePlus-Saude-IoT](https://github.com/Ven900/Sprint4_CarePlus_Saude_IoT.git)

### Simulação Wokwi

Protótipo virtual desenvolvido para testes e validação do sistema:

* Wokwi:[ https://wokwi.com/projects/465853181001403393](https://wokwi.com/projects/465853181001403393)

### Vídeo de Demonstração

Vídeo apresentando o funcionamento do sistema, arquitetura e resultados obtidos:

* YouTube: https://youtu.be/SEU-LINK-AQUI

---

## 📄 Documentação

O projeto contém:

Código-fonte do ESP32
Circuito desenvolvido no Wokwi
Bibliotecas utilizadas
Relatório técnico
Manual de execução
Vídeo demonstrativo
---

## 📚 Disciplina

**Edge Computing & Computer Systems**

### Sprint 3 — 2025

---

## 👥 Equipe

| Integrante           | RM     |
| -------------------- | ------ |
| Bruno Ventura        | 568316 |
| Diogo Henrique       | 568541 |
| Giovanna P. Zagaroli | 567572 |
| Venício Silva        | 568088 |
| Vinicius Nathan      | 567105 |

A equipe foi responsável pelo planejamento, desenvolvimento, integração e validação da solução CarePlus Saúde, aplicando conceitos de Internet das Coisas (IoT), Edge Computing, sistemas embarcados e monitoramento inteligente de dados voltados para a área da saúde.

---

## 🏛️ Instituição

**FIAP – Faculdade de Informática e Administração Paulista**

---

## 📌 Conclusão

O projeto CarePlus Saúde demonstra a aplicação prática dos conceitos de Internet das Coisas (IoT) e Edge Computing no contexto da saúde, possibilitando o monitoramento de sinais vitais de forma simples, acessível e eficiente.

A solução integra hardware, software e comunicação de dados em tempo real, permitindo a coleta, transmissão e visualização de informações relevantes para o acompanhamento de pacientes.

Além dos aspectos técnicos, o desenvolvimento do projeto contribuiu para o fortalecimento das competências da equipe em sistemas embarcados, comunicação MQTT, integração com Node-RED, trabalho colaborativo e desenvolvimento de soluções inovadoras voltadas para problemas reais.

Dessa forma, o CarePlus Saúde evidencia como a tecnologia pode ser utilizada para apoiar processos de monitoramento e tomada de decisão, reforçando a importância da IoT na transformação digital da área da saúde.

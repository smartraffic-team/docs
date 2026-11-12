# SmartTraffic — Documentação Técnica

!!! info "Sobre este documento"
    Documentação técnica oficial do **SmartTraffic**, protótipo acadêmico de
    controle semafórico adaptativo com visão computacional e integração com Arduino.

## O que é o SmartTraffic

O **SmartTraffic** é um sistema de controle de tráfego inteligente que utiliza
**visão computacional** (YOLO + OpenCV) para detectar veículos e pedestres em
tempo real, controlando semáforos de forma **autônoma** via integração com
**Arduino**.

O sistema foi desenvolvido para **otimizar a mobilidade urbana**: em vez de
temporização fixa, o estado do semáforo é decidido dinamicamente com base na
presença de agentes no cruzamento, com **limiar de ativação** para evitar
trocas constantes de estado e **alternância por inatividade** após períodos
sem detecções.

## Como funciona (visão de alto nível)

```mermaid
flowchart LR
    A[Webcam] -->|frames| B[Notebook<br/>Python + YOLO]
    B -->|comandos seriais| C[Arduino]
    C -->|aciona| D[Semáforo físico]
    B -->|status/contadores| E[Interface Web Local]
    E -->|modo manual| B
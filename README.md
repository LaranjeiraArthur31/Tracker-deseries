# Tracker-de-Séries
'''mermaid
  U([👤 Usuário]) --> FE[Frontend Web / App]

    FE --> AUTH[Autenticação\nJWT / OAuth]
    FE --> TRACK[Módulo de Tracking\nAdicionar / avaliar séries]
    FE --> MOOD[Módulo de Humor\nSelecionar estado emocional]
    FE --> NOTIF[Central de Notificações]

    TRACK --> DB[(Banco de Dados\nPostgreSQL)]
    AUTH  --> DB
    MOOD  --> REC[Motor de Recomendação\nIA + filtros]
    REC   --> DB

    REC   --> EXT_AI[API de IA\nOpenAI / Claude]
    TRACK --> EXT_TV[API de Séries\nTMDb / TVMaze]

    NOTIF --> SCHED[Scheduler\nVerificação periódica]
    SCHED --> EXT_TV
    SCHED --> DB
    SCHED --> PUSH[Serviço de Push\nEmail / Web Push]

    style U fill:#e1f5ee,stroke:#0f6e56,color:#085041
    style EXT_AI fill:#faeeda,stroke:#854f0b,color:#633806
    style EXT_TV fill:#faeeda,stroke:#854f0b,color:#633806
    style DB fill:#eeedfe,stroke:#534ab7,color:#3c3489
    style PUSH fill:#e6f1fb,stroke:#185fa5,color:#0c447c

## Sobre o Projeto
**Projeto:** [Tracker de Séries]
**Problema que resolve:** [Notificar novos episódios e lançamentos]

## Integrantes
| Nome | GitHub |
|------|--------|
| Arthur Lopes Laranjeira | @LaranjeiraArthur31 |
| Igor Mastrangelo Domingos | @IgorMastrangelo |
| Vitor Martins Furlan | @vtr1812 |


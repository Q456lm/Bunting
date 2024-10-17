```mermaid
    sequenceDiagram
    participant Attacker
    participant BotNet
    participant Firewall
    participant WebServer
    Attacker->>BotNet: Puts together Botnet
    Attacker->>BotNet: Tells Botnet what to attack
    Firewall->>BotNet: Attempts to Defend
    BotNet->>WebServer: Attacks Webserver
```
graph TB
    A[User] -->|Authentication| B[System]
    B -->|Manages| C[Devices]
    C -->|Controls| D[Device Scheduler]
    D -->|Schedules| E[Device]
    B -->|Triggers Notifications| F[Notification System]
    E --> F
    C --> F
    D --> F
    A -->|Receives Alerts| F
    B -->|Voice Commands| G[Voice Assistant]
    G -->|Commands| C

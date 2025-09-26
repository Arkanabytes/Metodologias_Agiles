
flowchart TD
    A[🚀 Inicio de la App] --> B{¿Usuario autenticado?}
    
    B -->|No| C[📱 Pantalla de Login]
    C --> D[📧 Ingreso Email/Password]
    C --> E[🌐 Login Social Google/Facebook]
    D --> F{¿Credenciales válidas?}
    E --> F
    F -->|No| G[❌ Error de autenticación]
    G --> C
    F -->|Sí| H[✅ Login exitoso]
    
    B -->|Sí| I[🏠 Pantalla Principal]
    H --> I
    
    I --> J[📊 Mostrar aforo gimnasio]
    I --> K[📈 Estadísticas usuario]
    I --> L[🎯 Objetivo actual]
    
    I --> M{Navegación}
    
    M -->|Hamburguesa ☰| N[📋 Menu Lateral]
    N --> O[👤 Mi Perfil]
    N --> P[📅 Reservas]
    N --> Q[📊 Mi Progreso]
    N --> R[💬 Chat Entrenador]
    N --> S[🤖 Asistente IA]
    N --> T[🥗 Plan Nutricional]
    N --> U[🚪 Cerrar Sesión]
    
    M -->|Botón Inferior| V[🏠 Inicio]
    M -->|Botón Inferior| W[📅 Reservas]
    M -->|Botón Inferior| X[📊 Progreso]
    M -->|Botón Inferior| Y[💬 Chat]
    M -->|Botón Inferior| Z[👤 Perfil]
    
    %% Página de Perfil
    O --> O1[🖼️ Avatar usuario]
    O --> O2[📝 Editar información]
    O --> O3[💳 Métodos de pago]
    O --> O4[🎯 Mis objetivos]
    O --> O5[⚙️ Configuración]
    O --> O6[📱 Conectar wearables]
    
    %% Página de Reservas
    P --> P1[📋 Lista clases disponibles]
    P1 --> P2{¿Hay espacios?}
    P2 -->|Sí| P3[✅ Reservar clase]
    P2 -->|No| P4[⏳ Lista de espera]
    P3 --> P5[🔔 Notificación confirmación]
    P4 --> P6[🔔 Notificación lista espera]
    
    %% Página de Progreso
    Q --> Q1[📈 Peso corporal]
    Q --> Q2[💪 Métricas de fuerza]
    Q --> Q3[🏃‍♂️ Cardio y calorías]
    Q --> Q4[📊 Barras de progreso]
    
    %% Chat con Entrenador
    R --> R1[💬 Historial mensajes]
    R1 --> R2[✍️ Escribir mensaje]
    R2 --> R3[📤 Enviar mensaje]
    R3 --> R4[🤖 Respuesta automática entrenador]
    R4 --> R1
    
    %% Asistente IA
    S --> S1{Tipo de consulta}
    S1 -->|💪| S2[Crear rutina personalizada]
    S1 -->|💡| S3[Consejos entrenamiento]
    S1 -->|🔥| S4[Motivación diaria]
    S1 -->|🥗| S5[Consejos nutricionales]
    S2 --> S6[🤖 Respuesta IA contextual]
    S3 --> S6
    S4 --> S6
    S5 --> S6
    
    %% Plan Nutricional
    T --> T1{Tipo de dieta}
    T1 -->|🎯| T2[Plan Definición]
    T1 -->|💪| T3[Plan Volumen/Masa muscular]
    T1 -->|⚖️| T4[Plan Pérdida de peso]
    T2 --> T5[🍽️ Menú diario con calorías]
    T3 --> T5
    T4 --> T5
    
    %% Funcionalidades en tiempo real
    J --> J1[🔄 Actualización automática cada 10s]
    J1 --> J2{Estado del gimnasio}
    J2 -->|<50%| J3[🟢 Normal]
    J2 -->|50-80%| J4[🟡 Ocupado]
    J2 -->|>80%| J5[🔴 Muy ocupado]
    
    %% Cerrar sesión
    U --> U1[🔓 Logout]
    U1 --> A
    
    %% Estilos
    classDef loginClass fill:#667eea,stroke:#333,stroke-width:2px,color:#fff
    classDef mainClass fill:#4caf50,stroke:#333,stroke-width:2px,color:#fff
    classDef featureClass fill:#ff9800,stroke:#333,stroke-width:2px,color:#fff
    classDef aiClass fill:#9c27b0,stroke:#333,stroke-width:2px,color:#fff
    classDef errorClass fill:#f44336,stroke:#333,stroke-width:2px,color:#fff
    classDef successClass fill:#2196f3,stroke:#333,stroke-width:2px,color:#fff
    
    class A,C,D,E loginClass
    class I,V,W,X,Y,Z mainClass
    class O,P,Q,R,T featureClass
    class S,S1,S2,S3,S4,S5,S6 aiClass
    class G,U1 errorClass
    class H,P3,P5 successClass








# Metodologias_Agiles
Proyecto que ayuda a ver como funciona la metodologia Scrum, con un proyecto simulador

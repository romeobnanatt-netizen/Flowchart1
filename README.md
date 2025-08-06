# Flowchart1
Flowchart
```mermaid
flowchart TD
  A[👋 Hi there! Welcome to Jubilant MotorWorks Chennai.\nReady to explore your next ride?] --> B1[🚗 Take a Quick Tour]
  A --> B2[❤️ Tell Me Why I’ll Love Mahindra]
  A --> B3[🏁 Book a Test Drive Today]

  %% Quick Tour Branch
  B1 --> C1[Which body style catches your eye?]
  C1 --> |Bold SUV| D1[XUV700, Scorpio-N]
  C1 --> |Rugged Cruiser| D2[Thar]
  C1 --> |Urban Hatch| D3[Glanza]
  C1 --> |Electric Future| D4[Born EV]

  D1 --> E1[▶️ Show 30s Video Highlight?]
  E1 --> |Yes| F1[Play Video then → “Impressive! Want to feel it live?”]
  E1 --> |Skip to Test Drive| G1[Branch to Test Drive Node]

  F1 --> |Book Test Drive| G1
  F1 --> |Tell Me More Teasers| H1[Sneak Peek Teaser:\n– 0–100 in <10s ⚡\n– Panoramic Sunroof ☁️\n– Alexa Integration 🔊\nBook a Test Drive?]

  H1 --> |Book Test Drive| G1
  H1 --> |Back to Menu| A

  %% Tell Me Why Branch
  B2 --> C2[Which matters most?]
  C2 --> |Power & Performance| D5[Diesel torque 💪]
  C2 --> |Comfort & Tech| D6[Heated seats + 12" screen 🎛️]
  C2 --> |Style & Presence| D7[Striking design ✨]

  D5 --> E2[“Feel that torque firsthand?”]
  E2 --> |Yes—Test Drive| G1
  E2 --> |Another Highlight| I1[Show next highlight → back to E2]

  D6 --> E3[“Fancy a spin to feel the comfort?”]
  E3 --> |Book Test Drive| G1
  E3 --> |Back to Menu| A

  D7 --> E4[“See it in person?”]
  E4 --> |Book Test Drive| G1
  E4 --> |Back to Menu| A

  %% Book Test Drive Branch
  B3 --> C3[Which model?]
  C3 --> |XUV700| D8
  C3 --> |Thar| D9
  C3 --> |Scorpio-N| D10
  C3 --> |Surprise Me| D11

  D8 --> E5[When suits you?]
  E5 --> |This Weekend| F2
  E5 --> |Next Week| F2
  E5 --> |I'm Flexible| F2

  F2 --> G2[“Just one more step—your name & best number?”]
  G2 --> H2[Booking Confirmed! 🎉 We'll call soon to lock it in.]

  %% Soft-Exit & Drop-off Hooks
  subgraph DropOffs
    X1((User hesitates))
    X2((User types unknown text))
    X3((User taps “Back to Menu”))
  end

  X1 --> Y1[“Would you like pics instead?”]
  Y1 --> |Yes| Z1[📸 Show Gallery then → “Intrigued? Book Test Drive”]
  Y1 --> |No| A

  X2 --> Y2[“Sorry, didn’t catch that. Try…”]
  Y2 --> A

  X3 --> Y3[“Keep you posted monthly?”]
  Y3 --> |Yes| Z2[“Great—we’ll send updates!”]
  Y3 --> |No| A

  %% Common Test Drive anchor
  G1 --> G2

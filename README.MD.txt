README.MD

# XLAN – The Smart Azure-Based Platform for Xbox LAN Events 🎮☁️

**XLAN** is an open-source cloud application built on Microsoft Azure that enables officially approved Xbox LAN events using a single Game Pass Ultimate license (where permitted). It streamlines participant registration, device validation, and license tracking, while providing real-time tools for event management — all while staying within Microsoft’s licensing guidelines.

---

## 🚀 Features

- 🎟️ **Participant Check-In** via Microsoft Account (Entra ID)
- 🕹️ **Xbox Console Linking** with local session registration
- ⏲️ **Game Time Management** and slot-based access
- 🔐 **License Validation** (planned integration with Xbox Live APIs)
- 📊 **Admin Dashboard** for live monitoring of session status
- 🛠️ Powered entirely by **Azure Functions**, **Cosmos DB**, and **Blazor WebAssembly**

---

## 🧱 Project Structure



/xlan ├── /client # Frontend built with Blazor WebAssembly │ ├── Pages/ # UI pages like Join.razor, EventView.razor │ └── Program.cs ├── /api # Azure Function App │ ├── EventRegister.cs │ └── DeviceStatus.cs ├── /shared # Shared models │ └── EventParticipant.cs ├── README.md # You're here! └── host.json # Azure Function config





---

## 🔧 Prerequisites

- [.NET 7 SDK](https://dotnet.microsoft.com/en-us/download)  
- [Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)  
- [Azure Functions Core Tools](https://learn.microsoft.com/en-us/azure/azure-functions/functions-run-local)  
- A valid **Azure Subscription**  
- Microsoft Entra ID (formerly Azure AD) App Registration  
- Cosmos DB instance (or use Azure Table Storage/SQL for demo)

---

## 📦 Getting Started

1. **Clone the repo**
   ```bash
   git clone https://github.com/your-username/xlan.git
   cd xlan



Deploy the Azure Function

bash
cd api
func start
Run the Blazor frontend

bash
cd client
dotnet run
Set environment variables or use local.settings.json for:

Cosmos DB Connection String

Xbox API Key (future integration)

Entra Tenant ID & Client ID

🛣️ Roadmap
✅ MVP Registration & Game Time UI

🚧 Xbox API validation integration

⏱️ Session timers and auto-kick

📡 SignalR-based live tracking

📋 Admin panel and usage reporting

📢 Partner onboarding & deployment templates

🤝 Contributing
Pull requests and forks welcome! If you're interested in helping shape the future of licensed multiplayer events, this is your place. Just fork, code, and PR.

📝 License
MIT License — free for community and educational use. Xbox-related features may require Microsoft developer consent or partnership.

📬 Contact
Developed by: Michael Münster 📧 thegeekdiarys@gmail.com 📍 Austria

> Built for gamers. Powered by Azure. Supported by community.




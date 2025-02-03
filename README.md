# LearnLab 🚀 <sub><sup>_Enhancing Learning Through Interactive Journeys_</sup></sub>

[![Open in CodeSpaces](https://img.shields.io/badge/Open%20in-CodeSpaces-blue?logo=visualstudiocode)](https://github.com/DAMG7245-Big-Data-Sys-SEC-02-Fall24/LearnLab)
[![Live Demo](https://img.shields.io/badge/Demo-Live%20Application-brightgreen)](http://34.45.163.161:3000/)
[![Swagger Docs](https://img.shields.io/badge/API-Swagger%20Docs-orange)](http://34.45.163.161:8000/docs)
[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.68.0+-00a393?logo=fastapi)](https://fastapi.tiangolo.com/)
[![Next.js](https://img.shields.io/badge/Next.js-13.0+-black?logo=next.js)](https://nextjs.org/)

<div align="center">
  <img src="https://via.placeholder.com/1200x400.png?text=LearnLab+Interactive+Learning+Platform" alt="LearnLab Banner">
</div>

## 🎯 Key Features

| Feature | Description | Tech Stack |
|---------|-------------|------------|
| 🎙️ Smart Podcasts | AI-generated audio content from PDFs with dramatic narration | OpenAI, 11 Labs |
| 📚 Adaptive Flashcards | Context-aware flashcards with spaced repetition | Pinecone, Gemini 1.5 |
| 🧠 Intelligent Quizzes | Dynamic question generation with analytics | LangGraph, PyPDF |
| ✍️ Content Conversion | Automated blog/social media post generation | Vercel AI SDK |

## 🚀 Quick Start

```bash
# Clone with submodules
git clone --recurse-submodules https://github.com/DAMG7245-Big-Data-Sys-SEC-02-Fall24/LearnLab

# Start core services
docker-compose up -d backend frontend db 

# Verify installation
curl http://localhost:8000/healthcheck
```

## 🏗️ System Architecture

```mermaid
flowchart LR
  A[User] --> B{Authentication}
  B -->|Success| C[Learning Dashboard]
  C --> D[Content Processing]
  D --> E[AI Services]
  E --> F[Learning Analytics]
```

## 📦 Project Structure

```
LearnLab/
├── frontend/          # Next.js 13 App Router
│   ├── app/          # Page routes
│   └── lib/          # Shared utilities
├── backend/          # FastAPI microservices
│   ├── core/         # Domain logic
│   └── api/          # REST endpoints
└── airflow/          # Data pipelines
```

## 🚢 Deployment

| Environment | Command | Port |
|-------------|---------|------|
| Development | `docker-compose up --build` | 3000 |
| Production | `docker-compose -f prod.yml up` | 80 |

Monitor services:
```bash
docker-compose logs -f --tail=100
```

## 🤝 Contributing

We welcome contributions! Check out our [contribution guidelines](CONTRIBUTING.md).

**Good First Issues:**
- [ ] Add dark mode support 🌓
- [ ] Implement mobile app integration 📱 
- [ ] Enhance PDF parsing accuracy 📄

## 📜 License

MIT Licensed - See [LICENSE](LICENSE) for details.

---

<div align="center">
  Made with ❤️ by Team LearnLab
  
  [Live Demo](http://34.45.163.161:3000/) | [Documentation](https://codelabs-preview.appspot.com/?file_id=1uRDRgIq0stv5MiOj-4f0KLE3mzC15eOw9zI4dzttLGg#0)
</div>

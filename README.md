```cpp
#include <iostream>
#include <vector>
#include <map>
using namespace std;

class AnishSolanki {
public:

    // ── Identity ──────────────────────────────────────────────────────────
    string name       = "Anish Solanki";
    string degree     = "BTech in AI & Data Science";
    string college    = "ADGIPS, Delhi (Affiliated to GGSIPU)";
    string location   = "India 🇮🇳";
    string github     = "github.com/TheAnishSolankii";

    // ── Skills used in RAG Chatbot Project ────────────────────────────────
    map<string, vector<string>> projectSkills = {
        {
            "Backend", {
                "Python", "FastAPI", "LangChain",
                "OpenAI GPT-4.1", "JWT Authentication",
                "SQLAlchemy", "FAISS Vector Database",
                "PyMuPDF", "REST APIs", "SSE Streaming",
                "Rate Limiting", "Docker"
            }
        },
        {
            "Frontend", {
                "React 18", "Tailwind CSS", "Vite",
                "React Router", "Axios", "React Markdown",
                "Context API", "Custom Hooks"
            }
        },
        {
            "AI & ML", {
                "RAG (Retrieval Augmented Generation)",
                "Vector Embeddings", "Semantic Search",
                "Text Chunking", "Prompt Engineering",
                "Conversation Memory"
            }
        },
        {
            "DevOps", {
                "Docker Compose", "Nginx",
                "GitHub Actions CI/CD", "Linux"
            }
        },
        {
            "CS Fundamentals", {
                "C++ DSA", "Binary Search", "Recursion",
                "Linked Lists", "Stacks & Queues",
                "OOP", "Data Structures"
            }
        }
    };

    // ── Currently Learning ────────────────────────────────────────────────
    vector<string> currentlyLearning = {
        "Advanced DSA in C++",
        "System Design",
        "Machine Learning",
        "Cloud Deployment (AWS / Railway)"
    };

    // ── Goals ─────────────────────────────────────────────────────────────
    vector<string> goals = {
        "Top-tier Tech Internship 🎯",
        "Crack DSA & System Design Interviews 💡",
        "Build real-world AI products 🤖",
        "1Cr+ package 🚀"
    };

    // ── Featured Project ──────────────────────────────────────────────────
    struct Project {
        string name;
        string description;
        vector<string> techStack;
        string link;
    };

    vector<Project> projects = {
        {
            "RAG Chatbot",
            "Production-ready AI chatbot — upload any PDF and chat with it using GPT-4.1. Features streaming responses, source citations, JWT auth, admin panel, vector search, and Docker deployment.",
            {
                "Python", "FastAPI", "LangChain", "FAISS",
                "OpenAI", "React", "Tailwind CSS", "Docker"
            },
            "github.com/TheAnishSolankii/rag-chatbot"
        }
    };

    // ── Greet ─────────────────────────────────────────────────────────────
    void greet() {
        cout << "┌─────────────────────────────────────────┐" << endl;
        cout << "│     Hey! I'm Anish — AI/DS Student      │" << endl;
        cout << "│     from ADGIPS, Delhi 🎓               │" << endl;
        cout << "│     Let's build something amazing 🔥    │" << endl;
        cout << "└─────────────────────────────────────────┘" << endl;
    }

    void printSkills() {
        cout << "\n🛠  Skills from RAG Chatbot Project:\n" << endl;
        for (auto& category : projectSkills) {
            cout << "  [" << category.first << "]" << endl;
            for (auto& skill : category.second) {
                cout << "    → " << skill << endl;
            }
            cout << endl;
        }
    }

    void printGoals() {
        cout << "\n🎯  Goals:\n" << endl;
        for (auto& goal : goals) {
            cout << "   ✦  " << goal << endl;
        }
        cout << endl;
    }
};

int main() {
    AnishSolanki me;
    me.greet();
    me.printSkills();
    me.printGoals();
    return 0;
}// paste the entire code above here
```

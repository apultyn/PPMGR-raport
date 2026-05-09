# PPMGR Raport

## Techniczne notatki

- *kilka* stron
- na pewno opisać technologię
- raczej skupić się na sytuacji na rynku niż w konkretne pomysły na pracę
    - istniejące badania bezpieczeństwa, podatności OWASP
- można wrzucić potencjalny test-bed
- na koniec można dać potencjalne kierunki rozwoju

## Research

### Ciekawe elementy

- [Blender MCP](https://www.blender.org/lab/mcp-server/)
- [Książka o bezpieczeństwie MCP](https://www.google.pl/books/edition/Cyber_Security_Adopting_the_Model_Contex/lLqeEQAAQBAJ?hl=pl&gbpv=1&dq=mcp+protocol&pg=PT17&printsec=frontcover)

### OWASP

- OWASP - *Open Worldwide Application Security Project*
- ze zwykłego top 10 narodził się projekt [OWASP GenAI Security Project](https://genai.owasp.org/)
    - [Manifest projektu](https://genai.owasp.org/project-mission-and-charter/)
- z tego powstał projekt mcp-top-10
- [GitHub](https://github.com/OWASP/www-project-mcp-top-10/blob/main/index.md)
- na dzień 26.04.2026 jest on w fazie beta - wypuszczono pierwsze top 10, zbierają feedback od społeczności
- następnymi krokami jest wypuszczenie finalnej wersji Top 10 podatności, a następnie cykliczne jej aktualizowanie
- w kontekście pracy - badany rodzaj podatności (*Tool Poisoning*) jest na 3 miejscu rankingu, a tego typu podatność może być wykorzystana do ataków opisanych w topkach OWASPU

### MCP

- [Dokumentacja MCP](https://modelcontextprotocol.io/docs/getting-started/intro)
- 3 kluczowe koncepty do potencjalnego zbadania:
    - *Resources* - "plikowe" dane odczytywane przez klientów
    - *Tools* - funkcje wołane przez LLM
    - *Prompts* - templaty pomagające użytkownikowi wykonać jakieś zadanie
- praca się skupia na *Tools*, natomiast dobre do wstępu teoretycznego

### Artykuły

- [A Comprehensive Survey on Model Context Protocol: Architecture, Tool Integration, and the Future of AI Interoperability](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=5957238) - bardziej opis samego konceptu MCP
- [MCPTox: A Benchmark for Tool Poisoning Attack on Real-World MCP Servers](https://arxiv.org/pdf/2508.14925) - zbadali 353 realnych narzędzi, skuteczność ataków wyniosła 72,8% !!!
    - trochę inne rodzaje opisów, same prompt injection

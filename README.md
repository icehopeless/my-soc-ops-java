🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

# Soc Ops

**Soc Ops** é um jogo de social bingo para encontros presenciais. 
Descubra rapidamente pessoas que combinam com prompts divertidos e ganhe com uma linha completa de conexões.

> 🎯 Um playground leve para explorar Spring Boot, frontend web e lógica de jogo com foco em experiência social.

---

## 💡 Por que abrir este projeto?

- **Jogo social simples**: tabuleiro 5×5 com prompts de icebreaker.
- **Experiência interativa**: célula central "FREE SPACE" já marcada e uma interface pronta para conectar pessoas.
- **Arquitetura moderna**: backend Spring Boot + Thymeleaf + frontend leve.
- **Aprendizado prático**: ideal para workshops, demos e protótipos colaborativos.

---

## 🚀 O que o projeto faz

- Serve uma página web em `/`
- Gera um tabuleiro novo em `/api/bingo/fresh-board`
- Monta cada carta com 24 prompts aleatórios + célula central gratuita
- Detecta vitória com linhas, colunas e diagonais completas
- Mantém a lógica de jogo encapsulada em `BoardAssembler`

---

## ✨ Destaques

- `socops/src/main/java/com/socops/data/IcebreakerPrompts.java` — banco de prompts
- `socops/src/main/java/com/socops/service/BoardAssembler.java` — montagem e vitória
- `socops/src/main/java/com/socops/web/BingoRestController.java` — API e rota de página
- `socops/src/main/resources/templates/game.html` — interface do jogo
- `socops/config/checkstyle/checkstyle.xml` — regras de lint e estilo

---

## ▶️ Rápido start

```bash
cd socops
./mvnw spring-boot:run
```

Depois, acesse: `http://127.0.0.1:8080`

---

## 🛠️ Build e teste

```bash
cd socops
./mvnw clean package
./mvnw test
```

---

## 📚 Workshop e guia

Explore o passo a passo em:

- `workshop/GUIDE.md`
- `workshop/00-overview.md`
- `workshop/01-setup.md`
- `workshop/02-design.md`
- `workshop/03-quiz-master.md`
- `workshop/04-multi-agent.md`

---

## 🤝 Contribuição

1. Clone o repositório
2. Use `./socops/mvnw test`
3. Envie PRs com melhorias de jogo, UI ou integração

---

## 💬 Curiosidade

O app também pode ser usado como base para criar outros jogos de tabuleiro social, experiências de onboarding ou dinâmicas de integração em equipes.

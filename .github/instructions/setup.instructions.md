---
description: Workspace setup guidance for the my-soc-ops-java Spring Boot project.
---

# Workspace Setup Instructions

## Mandatory development checklist
- [ ] lint (if applicable)
- [ ] build: `./socops/mvnw clean package`
- [ ] test: `./socops/mvnw test`

## Key info
- Root app: `socops/`
- Maven entry: `socops/pom.xml`
- Backend code: `socops/src/main/java/com/socops/`
- UI entry: `socops/src/main/resources/templates/game.html`
- Styles: `socops/src/main/resources/static/css/app.css`

## Runtime
- Requires Java 21 and the Maven wrapper.
- Start with `./socops/mvnw spring-boot:run`.
- App should listen on `http://127.0.0.1:8080`.

## VS Code task hints
- `mvn: run` to launch
- `mvn: build` to package
- `mvn: test` to verify

## Contributor note
Use `socops` as the Maven working directory; keep UI work in Thymeleaf/CSS and backend logic inside `service/` and `web/`.

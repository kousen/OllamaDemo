# Ollama Demo

A simple Spring Boot application demonstrating integration with [Ollama](https://ollama.ai/) using Spring AI.

## Prerequisites

- Java 21+
- [Ollama](https://ollama.ai/) installed and running locally
- A model pulled in Ollama (default: `gpt-oss`)

## Setup

1. Install Ollama from https://ollama.ai/
2. Pull the model:
   ```bash
   ollama pull gpt-oss
   ```
3. Ensure Ollama is running (default: http://localhost:11434)

## Configuration

The application is configured in `src/main/resources/application.properties`:

```properties
spring.application.name=OllamaDemo
spring.ai.ollama.chat.model=gpt-oss
```

Change the model name to use a different Ollama model.

## Running

```bash
./gradlew bootRun
```

## Testing

The demo includes a test that sends a prompt to the Ollama model:

```bash
./gradlew test
```

## Dependencies

- Spring Boot 3.5.8
- Spring AI 1.1.0 (Ollama integration)
- JUnit 5

## License

MIT License - see [LICENSE](LICENSE) for details.

# llama-index OpenInference instrumentation example

This is a [LlamaIndex](https://www.llamaindex.ai/) project bootstrapped with [`create-llama`](https://github.com/run-llama/LlamaIndexTS/tree/main/packages/create-llama) and instrumented using OpenInference.

Our example will export spans data to [arize-phoenix](https://github.com/Arize-ai/phoenix), however you can run your code anywhere and can use any exporter that OpenTelemetry supports.

## Getting Started with Local Development

First, startup the backend as described in the [backend README](./backend/README.md).

Second, run the development server of the frontend as described in the [frontend README](./frontend/README.md).

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Getting Started with Docker-Compose

If you'd like, add your own PDFs to `./backend/data` to build indexes over.

Either create a `.env` file that contains an OpenAI API key or set the `OPENAI_API_KEY` env variable.

Ensure that Docker is installed and running. Run the command `docker compose up` to spin up services for the frontend, backend, and Phoenix. Once those services are running, open [http://localhost:3000](http://localhost:3000) to use the chat interface. When you're finished, run `docker compose down` to spin down the services.

Traces can be viewed using the [Phoenix UI](http://localhost:6006).

## Learn More

To learn more about LlamaIndex, take a look at the following resources:

-   [LlamaIndex Documentation](https://docs.llamaindex.ai) - learn about LlamaIndex (Python features).
-   [LlamaIndexTS Documentation](https://ts.llamaindex.ai) - learn about LlamaIndex (Typescript features).

You can check out [the LlamaIndexTS GitHub repository](https://github.com/run-llama/LlamaIndexTS) - your feedback and contributions are welcome!
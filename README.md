<div align="center">
<img src="./docs/images/head-cover.png" alt="icon"/>
<h1 align="center">NextChat (ChatGPT Next Web - 🐱 jalr4ever)</h1>
</div>

## Introduce

- See original repo: https://github.com/ChatGPTNextWeb/ChatGPT-Next-Web

## What's new

### Define a default model

To define a default model, simply add a `+*` prefix to `CUSTOM_MODELS` item. The first model to receive this prefix will become the new chat default model.

Each new chat window will use the default model, but old windows that have already changed the model will not be affected by this.

## Usage

Build image by yourself or just simple use `jalr4ever/chatgpt-next-web`, for example:

```shell
docker pull jalr4ever/chatgpt-next-web

docker run -d -p 3000:3000 \
   -e OPENAI_API_KEY=sk-xxxx \
   -e CODE=your-password \
   -e CUSTOM_MODELS=-all,+*gpt-4-1106-preview,+gpt-3.5-turbo,+gpt-3.5-turbo-0613,+gpt-4-0125-preview \
   jalr4ever/chatgpt-next-web
```

## LICENSE

[MIT](https://opensource.org/license/mit/)

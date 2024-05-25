# Morpheus

An AI-powered search engine UI. GPT4.

![capture](/public/capture-240404_blk.png)


### 1. Fork or Clone the repo

Fork the repo to your Github account, then run the following command to clone the repo:

```
https://github.com/Mulc1b3R/morpheus.git
```

### 2. Install dependencies

```
cd morpheus
npm  i
```

### 3. Fill out secrets

```
cp .env.local.example .env.local
```

Your .env.local file should look like this:

```
# Used to set the base URL path for OpenAI API requests.
# If you need to set a BASE URL, uncomment and set the following:
# OPENAI_API_BASE=

# Used to set the model for OpenAI API requests.
# If not set, the default is gpt-4-turbo.
# OPENAI_API_MODEL='gpt-4-turbo'

# OpenAI API key retrieved here: https://platform.openai.com/api-keys
OPENAI_API_KEY=[YOUR_OPENAI_API_KEY]

# Tavily API Key retrieved here: https://app.tavily.com/home
TAVILY_API_KEY=[YOUR_TAVILY_API_KEY]

# Only writers can set a specific model. It must be compatible with the OpenAI API.
# USE_SPECIFIC_API_FOR_WRITER=true
# SPECIFIC_API_BASE=
# SPECIFIC_API_KEY=
# SPECIFIC_API_MODEL=
```

_Note: This project focuses on Generative UI and requires complex output from LLMs. Currently, it's assumed that the official OpenAI models will be used. Although it's possible to set up other models, if you use an OpenAI-compatible model, but we don't guarantee that it'll work._

### 4. Run app locally

```
npm start dev
```

visit http://localhost:3000.

## 🌐 Deploy

Host your own live version of Morpheus with Vercel .

### Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fmiurla%2Fmorphic&env=OPENAI_API_KEY,TAVILY_API_KEY)


## ✅ Verified models

List of verified models that can be specified to writers.

- [Groq](https://console.groq.com/docs/models)
  - LLaMA3 8b
  - LLaMA3 70b

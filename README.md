# Morpheus 


An AI-powered search engine UI. GPT4.

![capture](/public/capture-240404_blk.png)

************************************************************************************************************************************
### 1. Fork or Clone the repo

 Clone the repo:

```
https://github.com/Mulc1b3R/morpheus.git
```

### 2. Install dependencies

```
cd morpheus
npm  i
```

### 3. Fill out .env

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

Note: This project uses gpt4 , which is much more expensive than 3.5 
and will 'drain' the credit on your api key up to 20 times faster.
GPT 3.5 is fine for everyday use...
Zendog : https://zendog-eight.vercel.app/


### 4. Run app locally

```
npm start dev
```

visit http://localhost:3000.

## 🌐 Deploy

Host your own live version of Morpheus with Vercel .

### Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fmiurla%2Fmorphic&env=OPENAI_API_KEY,TAVILY_API_KEY)


*************************************************************************************************************************

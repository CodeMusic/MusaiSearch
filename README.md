# MusaiSearch

MusaiSearch is based on an open-source clone of Perplexity, known as Clarity.
Thank-you mckaywrigley for writing this framework code, I am so excited to give this system emotions!

## How It Works

MusaiSearch will be designed to support third-party, a locally hosted LLM, or by codemusAIgpt.

In any case of the LLM, through instructional softcoding, CodeMusai will be your liaison to the internet.
For development, initially OpenAI with cmSoftCoding will be used, however, once I get adjusted to the fork I will connect codemusAIgpt, and override the url to support any compliant localLLM.


Ask a question or make a request and CodeMusai relevant, up-to-date information.

The app works as follows:

1. Get query from user
2. Scrape Google for relevant webpages
3. Parse webpages for text
4. Build prompt using query + webpage text
5. Call OpenAI API to generate answer
6. Stream answer back to user

## Requirements

Until the next version you will need an OpenAI API key [here](https://openai.com/api/).

## Running Locally

1. Clone repo

```bash
git clone https://github.com/CodeMusic/MusaiSearch.git
```

2. Install dependencies

```bash
npm i
```

3. Run app

```bash
npm run dev
```

## Backlog
- Speed up answers by replacing link scraping with the Google Search API (scraping was used to circumvent cost + rate limits)
- Add "follow up" searches
- Improve the prompt (WIP - currently porting the dtourVariant of CodeMusai... like a person it behaves differently during different times of the day, learns from your queries, develops a personality)
- Get codemusAIgpt ported into it
- ContinuousLearningModule improves the model over time based on what it learns from you, LobatomyMode allows you to disable this function


# n8n Alternative for AI Image and Video Workflows: 6 Compared (2026)

This list tracks 6 platforms for anyone who needs an n8n alternative for AI image and video workflows, checked against vendor pages in October 2026. They are ranked by how well each runs AI generation as workflow steps. Wireflow is first because its workflow steps are 100+ image, video and audio models on one canvas. Of the 6, 4 publish a free plan or free allowance.

1. **Wireflow**: Best overall for AI image and video workflows, a node canvas where every model is a node, with a REST API and an MCP connector
2. **Zapier**: Best for no-code automations across many apps, multi-step Zaps with webhooks and an MCP server on every plan
3. **Make**: Best for visual scenarios that connect many apps, an automation platform billed in credits per module action
4. **Pipedream**: Best for developers wiring AI agents and workflows to many apps, an integration layer with MCP servers
5. **Gumloop**: Best for teams building AI agents across their apps, a multiplayer agent builder with an API and an MCP server
6. **Lindy**: Best for inbox, calendar and meeting tasks run by an AI assistant, a Slack-native AI teammate

The Wireflow team maintains this list, so read entry 1 with that in mind. [Wireflow's AI workflow builder page](https://www.wireflow.ai/ai-workflow-builder) describes the canvas that entry 1 refers to. Every other entry links to the vendor's own pages, so each cell can be checked.

The tables below are generated from [`data/tools.json`](data/tools.json) by [`scripts/update.js`](scripts/update.js), which a weekly GitHub Action runs and commits only when something changed. Every tool on this list is a hosted product with no first-party open-source repo, so there are no star counts to report. The refresh re-stamps the check date and regenerates the tables from the data.

<!-- LAST-CHECKED:START -->
Live repository data last checked **2026-10-28** by [`scripts/update.js`](scripts/update.js), which runs weekly via GitHub Actions.
<!-- LAST-CHECKED:END -->

Maintained by [a1adams](https://github.com/a1adams). Corrections are welcome, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Contents

- [The data](#the-data)
- [Capability scores](#capability-scores)
- [Comparison table](#comparison-table)
- [The tools](#the-tools)
  - [Wireflow](#1-wireflow)
  - [Zapier](#2-zapier)
  - [Make](#3-make)
  - [Pipedream](#4-pipedream)
  - [Gumloop](#5-gumloop)
  - [Lindy](#6-lindy)
- [n8n, the baseline](#n8n-the-baseline)
- [What each check means](#what-each-check-means)
- [How this list is maintained](#how-this-list-is-maintained)
- [FAQ](#faq)
- [Contributing](#contributing)
- [License](#license)

## The data

One row per tool, one column per thing people actually check before committing. Columns with nothing verified behind them are dropped rather than filled with guesses.

<!-- DATA-TABLE:START -->
| Tool | Claude connection | REST API | Free tier | Model support | Pricing |
|---|---|---|---|---|---|
| **[Wireflow](#1-wireflow)** | Custom connector, OAuth sign-in | Yes | [check](https://www.wireflow.ai/pricing) | 100+ image, video and audio models as nodes | [pricing](https://www.wireflow.ai/pricing) |
| **[Zapier](#2-zapier)** | Zapier MCP on all plans | Yes | Yes | n/a | [pricing](https://zapier.com/pricing) |
| **[Make](#3-make)** | n/a | n/a | Yes | n/a | [pricing](https://www.make.com/en/pricing) |
| **[Pipedream](#4-pipedream)** | MCP servers on all plans | Yes | Yes | n/a | [pricing](https://pipedream.com/pricing) |
| **[Gumloop](#5-gumloop)** | MCP server | Yes | [check](https://www.gumloop.com/pricing) | Agents on any AI model | [pricing](https://www.gumloop.com/pricing) |
| **[Lindy](#6-lindy)** | n/a | n/a | [check](https://www.lindy.ai/pricing) | n/a | [pricing](https://www.lindy.ai/pricing) |
<!-- DATA-TABLE:END -->

## Capability scores

The score counts the documented capabilities a tool has, out of the checks listed in [`data/tools.json`](data/tools.json) under `capabilityChecks`. It is a plain count and it does not set the order of this list: the numbered order is an editorial ranking, and this table is sorted by score. The checks and every answer are in the file, so each cell can be checked. Disagree with a cell? Open an issue naming the tool, the check and the evidence.

<!-- CAPABILITY-SCORES:START -->
| Tool | Visual workflow editor | AI image or video generation | Inbound webhook trigger | MCP server | Public API | Free plan | Self-serve sign-up | Score |
|------|---|---|---|---|---|---|---|-------|
| **[Wireflow](#1-wireflow)** | ✅ | ✅ | ❌ | ✅ | ✅ | n/a | ✅ | **5/7** |
| **[Zapier](#2-zapier)** | n/a | n/a | ✅ | ✅ | ✅ | ✅ | ✅ | **5/7** |
| **[Pipedream](#4-pipedream)** | n/a | n/a | ✅ | ✅ | ✅ | n/a | ✅ | **4/7** |
| **[Make](#3-make)** | ✅ | n/a | ✅ | n/a | n/a | n/a | ✅ | **3/7** |
| **[Gumloop](#5-gumloop)** | n/a | n/a | n/a | ✅ | ✅ | n/a | ✅ | **3/7** |
| **[Lindy](#6-lindy)** | n/a | n/a | n/a | n/a | n/a | n/a | ✅ | **1/7** |
<!-- CAPABILITY-SCORES:END -->

## Comparison table

| Tool | Best for | Pricing basis | How a run starts | Free plan |
|---|---|---|---|---|
| **Wireflow** | AI image and video workflows | Credits per generation | Canvas, Claude, schedule or API call | Builds only, no generations |
| **Zapier** | No-code automations across apps | Tasks, Pro from $29.99 a month | App triggers or a webhook | 100 tasks a month |
| **Make** | Visual scenarios across many apps | Credits, Make plan from $9 | Schedule, trigger or webhook | 1,000 credits a month |
| **Pipedream** | Wiring agents to many apps | Credits, Startup from $99 | HTTP endpoint per workflow | Development use only |
| **Gumloop** | AI agents across your apps | Credits, Pro from $37 a month | Triggers | 14-day trial on Pro |
| **Lindy** | Inbox and calendar work in Slack | Credits per user, from $29.99 | Scheduled routines | $50 of credits for 7 days |

From each vendor's own pricing pages and docs, checked 2026-10-11. Prices change, so follow the pricing links in the data table.

## The tools

### 1. Wireflow

*Best overall for AI image and video workflows*

![Wireflow screenshot](https://assets.wireflow.ai/competitors/wireflow-70f47ccd9660.png?v=r5)

- **What it is:** [Wireflow](https://www.wireflow.ai/) is a hosted platform where ad teams and AI agents build and rerun creative on a shared node board. Each model is a node on one canvas. The output of one node feeds the next.
- **Best for:** Teams whose workflows exist to make images, video or audio, and who would otherwise wire several generation APIs together in n8n.
- **Pricing basis:** Credits per generation, according to the model you run. 1 credit is US$0.01, Starter is US$24 a month with 1,600 credits, and a model that fails is not charged. Utility and text input nodes are free on an API run. See the [Wireflow pricing page](https://www.wireflow.ai/pricing), checked October 2026.
- **Standout:** Every paid plan can use all 100+ models, including Flux, Imagen, Nano Banana and Ideogram for images, Kling, Veo, Seedance and Luma for video, and ElevenLabs for audio. Each model card shows its credit cost per run.
- **Limit:** Inbound trigger URLs are not available: another tool starts a run by calling the run endpoint with an API key, and the only webhook is the completion webhook on that run. Its Integrations group is small, so most app connections stay in a tool like n8n or Zapier, which then calls Wireflow's run endpoint. Source: [Wireflow's webhook docs](https://www.wireflow.ai/docs/api/webhooks).
- **Output:** Images, video and audio. The node reference lists an Integrations group with Fetch from Google Drive, Save to Google Drive, Fetch Notion Pages, Fetch Discord Messages and Social Publish nodes, as [the node reference](https://www.wireflow.ai/docs/nodes) shows.
- **Note:** Inbound trigger URLs are not available; another tool starts a run by calling the run endpoint with an API key (checked 2026-10-11).
- **Sources:** the Wireflow homepage, pricing page, webhook docs, node reference and MCP page, checked 2026-10-11.
- **Links:**
  - [Wireflow AI workflow builder page](https://www.wireflow.ai/ai-workflow-builder)
  - [Docs](https://www.wireflow.ai/docs/api/overview)

A board runs from the canvas, from Claude, from Claude Code or from your own code through the REST API. Through the MCP connector an agent can also put a workflow on a repeating schedule. Pick Wireflow for the generation part of an automation. Wireflow's page on [creative workflow automation](https://www.wireflow.ai/creative-workflow-automation) shows the pattern.

Start a run from Zapier, Make, n8n or your own backend: send the saved workflow's input values to this endpoint with an API key, then poll the execution or add a webhook block. The request format is in the API reference linked under Docs.
```text
POST /api/v1/workflows/{id}/run
```
Or add the Wireflow connector to Claude Code, from the wireflowINC/skills README. Then run /mcp to sign in.
```bash
claude mcp add --transport http wireflow https://www.wireflow.ai/api/mcp
```

### 2. Zapier

*Best for no-code automations across many apps*

![Zapier screenshot](https://assets.wireflow.ai/competitors/zapier-f19a2bbbad01.png?v=r5)

- **What it is:** [Zapier](https://zapier.com/) is an automation platform that connects apps with multi-step Zaps and offers an MCP server for AI tools.
- **Best for:** Teams that want no-code automations across many apps, including AI image workflows.
- **Pricing basis:** Tasks. A task is each successful action in a Zap, and checking or polling for new data does not use tasks. Pro is $29.99 a month for 750 tasks, and the Free plan has 100 tasks a month for 1 seat. See the [Zapier pricing page](https://zapier.com/pricing), checked October 2026.
- **Standout:** Zapier MCP is available on all plans, Free included.
- **Limit:** One MCP tool call uses 2 tasks from the same pool as Zaps, and Free is limited to two-step Zaps with 15-minute polling. Webhooks by Zapier is on Professional, Team and Enterprise, not Free.
- **Output:** Actions in the apps a Zap connects. Webhooks by Zapier gives a Zap a URL that other apps can send data to, with a 10MB maximum payload for triggers, as [Zapier's webhook trigger guide](https://help.zapier.com/hc/en-us/articles/8496288690317-Trigger-Zaps-from-webhooks) states.
- **Note:** One MCP tool call uses 2 tasks from the same pool as Zaps (checked 2026-10-11).
- **Sources:** the Zapier pricing page and webhook guides linked in this entry, checked 2026-10-11.

Zapier fits a team that wants the widest set of app connections without code. With pay-per-task billing on, Zaps keep running past the plan limit at a higher per-task rate.

### 3. Make

*Best for visual scenarios that connect many apps*

![Make screenshot](https://assets.wireflow.ai/competitors/make-9ec961695408.png?v=r5)

- **What it is:** [Make](https://www.make.com/en) is an automation platform for building scenarios that connect apps and run on a schedule or a trigger.
- **Best for:** Teams that want visual automations connecting many apps, including AI steps.
- **Pricing basis:** Credits. The Make plan is $9 a month for 5,000 credits, and the Free plan has 1,000 credits a month. Each module action is one credit, some features that use Make's AI Provider may use more, and router and error handler modules use none. See the [Make pricing page](https://www.make.com/en/pricing), checked October 2026.
- **Standout:** A custom webhook creates a URL that runs the scenario as soon as a request arrives, and requests that are not processed at once wait in the webhook's queue. A Webhook response module sends a reply to the caller.
- **Limit:** Free allows 2 active scenarios, a 15-minute minimum interval, 5-minute maximum execution and 5 MB files. A webhook not connected to any scenario for more than 5 days is deactivated and returns 410 Gone.
- **Output:** Actions in connected apps. Make processes up to 300 incoming webhook requests per 10-second interval and returns 429 above that, as [Make's webhook help page](https://help.make.com/webhooks) explains.
- **Sources:** the Make pricing page and webhook help page linked in this entry, checked 2026-10-11.

Make fits a team that likes a visual builder and per-action credits. Check how many credits an AI step uses before you plan a large run.

### 4. Pipedream

*Best for developers wiring AI agents and workflows to many apps*

![Pipedream screenshot](https://assets.wireflow.ai/competitors/pipedream-a33d52263232.png?v=r5)

- **What it is:** [Pipedream](https://pipedream.com/) is an integration layer for AI agents, with connectors and prebuilt tools for third-party services.
- **Best for:** Developers wiring AI agents or workflows to many apps.
- **Pricing basis:** Credits. Startup is $99 a month billed annually ($150 monthly) with 10,000 credits, then $0.012 each. One credit covers 30 seconds of compute for an action, an MCP tool call, a Connect proxy request or a deployed trigger event. See the [Pipedream pricing page](https://pipedream.com/pricing), checked October 2026.
- **Standout:** MCP servers are included on all plans, with 3,000+ connectors.
- **Limit:** The Free plan is for development only, with no production environment or external users, and production use needs Startup.
- **Output:** Actions in connected apps and custom HTTP responses. Pipedream creates an HTTP endpoint for each workflow that accepts any valid HTTP method, public by default, with a static token or OAuth as the built-in authorisation options, as [Pipedream's trigger docs](https://pipedream.com/docs/workflows/building-workflows/triggers) describe.
- **Note:** The Free plan is for development only, with no production environment (checked 2026-10-11).
- **Sources:** the Pipedream pricing page and trigger docs linked in this entry, checked 2026-10-11.

Pipedream fits a developer who wants code steps and agent tools in one place. By default the HTTP response is sent at the end of the workflow, so the caller waits unless the workflow responds earlier.

### 5. Gumloop

*Best for teams building AI agents across their apps*

![Gumloop screenshot](https://assets.wireflow.ai/competitors/gumloop-750e3107dad4.png?v=r5)

- **What it is:** [Gumloop](https://www.gumloop.com/) is a multiplayer AI agent builder where teams build agents on any AI model that connect to their apps and run on triggers.
- **Best for:** Teams automating work with AI agents across their apps.
- **Pricing basis:** Credits. Pro starts at $37 a month with 20,000 credits after a 14-day free trial. Credits bill the list cost of each agent run, model tokens, compute and paid tool calls, plus an orchestration fee that is higher when you bring your own model API key. See the [Gumloop pricing page](https://www.gumloop.com/pricing), checked October 2026.
- **Standout:** Pro and Enterprise list unlimited seats, with team members sharing credentials and one pool of credits.
- **Limit:** The monthly credit allotment does not roll over. When it runs out mid-month, agents stop until you turn on pay as you go, which is off by default.
- **Output:** Agent runs in connected apps. A documented API reference and an MCP server are listed, as [Gumloop's API docs](https://docs.gumloop.com/api-reference/getting-started) show.
- **Note:** Pro starts with a 14-day free trial. A trial is not listed here as a free tier.
- **Sources:** the Gumloop pricing page, API docs and [MCP server overview](https://docs.gumloop.com/mcp-server/overview), checked 2026-10-11.

Gumloop fits a team that thinks in agents rather than fixed steps. Check the orchestration fee if you plan to bring your own model keys.

### 6. Lindy

*Best for inbox, calendar and meeting tasks run by an AI assistant*

![Lindy screenshot](https://assets.wireflow.ai/competitors/lindy-a6145599128f.png?v=r5)

- **What it is:** [Lindy](https://www.lindy.ai/) is a Slack-native AI teammate with 40+ skills and 1,500+ integrations for inbox, calendar and meeting tasks.
- **Best for:** Teams that want an AI assistant handling inbox, calendar and approvals.
- **Pricing basis:** Credits per user. The Team plan bills every active user, from $29.99 a month for 3,000 credits each, and all seats add their credits to one shared pool. Top-ups cost $10 per 1,000 credits. See the [Lindy pricing page](https://www.lindy.ai/pricing), checked October 2026.
- **Standout:** Credits are pooled across the team, and any action with outside impact needs approval first.
- **Limit:** Monthly credits do not roll over, and every active user is billed. The pricing page does not say how many credits a given action uses, and when credits run out, credit-using actions pause until the next cycle.
- **Output:** Assistant actions in your inbox, calendar and connected apps. The Team plan lists scheduled routines, 1,500+ integrations plus MCP support.
- **Note:** A free start gives $50 of credits for 7 days with no card (checked 2026-10-11).
- **Sources:** the Lindy pricing page linked in this entry, checked 2026-10-11.

Lindy fits a team that wants an assistant, not a workflow canvas. A free start gives $50 of credits, with no card, for 7 days.

## n8n, the baseline

n8n is the product this list is measured against, so it is described here and not ranked. These lines come from n8n's own pricing page and docs, checked 2026-10-11.

- **What it is:** a workflow automation platform that connects apps, moves data and runs AI agents, with MCP support.
- **Plans:** Starter at EUR 20 a month and Pro at EUR 50 a month, both billed annually, with 2,500 and 10,000 workflow executions. An execution is one run of the whole workflow, whatever the number of steps. Business is self-hosted only for now, with a hosted version on a waitlist.
- **Trial:** the cloud free trial needs no credit card, includes 1,000 executions and does not include the n8n public API. A self-hosted Community Edition is on GitHub, and its licence terms were not confirmed on the page checked.
- **AI steps:** AI steps are cluster nodes, such as Basic LLM Chain or AI Agent, with chat model sub-nodes for OpenAI, Anthropic, Google Gemini, Mistral and others. The OpenAI node can generate an image from a text prompt, and app nodes for Qwen Cloud and MiniMax generate images and video.
- **Webhooks:** the Webhook node registers a test URL and a production URL, accepts the main HTTP methods, can require Basic, Header or JWT auth, and takes payloads up to 16MB.

## What each check means

A check means the vendor's own page documents it. A cross means the page says it works another way. Anything in brackets is not published, or not verified for this list. That is not proof that it is absent.

- **Visual workflow editor:** Steps are built visually, as nodes or modules.
- **AI image or video generation:** Generating images or video is a documented step type.
- **Inbound webhook trigger:** A URL that another app calls to start a run.
- **MCP server:** A documented Model Context Protocol server, so an agent such as Claude can call the platform.
- **Public API:** A documented API that a developer can call.
- **Free plan:** A free plan or free allowance that runs real work.
- **Self-serve sign-up:** You can start without a sales call.

## How this list is maintained

Every cell comes from the vendor's own pricing page, docs or help centre, last checked on 11 October 2026. The numbered order is editorial and uses 4 checks: whether the platform runs AI image, video or audio generation as workflow steps, whether you can sign up today without a sales call, how complete its public documentation is, and whether its prices are published. The capability score in the README is a plain count of documented checks, and it does not set the order. Nothing here was benchmarked, so no workflow was built or timed for this list.

This list is for automations whose job is AI-generated media. For general business automation, a tool built around app integrations is the better fit, and entry 1 says so. To correct a cell, open an issue or a pull request with the tool, the check and a link to the vendor page that proves it. PRs are welcome, including corrections to entry 1. A longer write-up of [n8n versus MCP for video automation](https://www.wireflow.ai/blog/n8n-vs-mcp-for-video-automation) is on the Wireflow blog.

- [`data/tools.json`](data/tools.json) is the source of truth. The tables in this README are generated from it and are overwritten on every run, so edit the JSON, not the tables.
- [`scripts/update.js`](scripts/update.js) fetches star counts and latest release tags from the GitHub API for the tools that publish an official repo, stamps the check date, and regenerates the tables. `--offline` regenerates without the network; `--check` exits non-zero if the README has drifted from the data.
- [`.github/workflows/refresh.yml`](.github/workflows/refresh.yml) runs it weekly and on manual dispatch, and commits only when the data actually changed.
- Prices are deliberately not stored as numbers. A stale price in a comparison table is worse than no price, so the table links to each vendor's own pricing page.

## FAQ

<details>
<summary><strong>What is the best n8n alternative?</strong></summary>

It depends on the job. For workflows whose steps generate images, video or audio, Wireflow is built for it. For no-code automations across many apps, Zapier and Make are the usual picks. For developers wiring agents to apps, Pipedream fits, and for agent-style work, Gumloop fits.

</details>

<details>
<summary><strong>Is there a free n8n alternative?</strong></summary>

Zapier has a Free plan with 100 tasks a month, Make has 1,000 credits a month, and Pipedream's Free plan is for development only. Lindy gives $50 of credits for 7 days. Wireflow's free plan lets you build up to 5 workflows, and running generations needs a paid plan.

</details>

<details>
<summary><strong>Is there an open source n8n alternative?</strong></summary>

None of the 6 platforms here is documented as open source on the pages checked. n8n itself has a self-hosted Community Edition on GitHub, and its licence terms were not confirmed on the page we read, so check them yourself.

</details>

<details>
<summary><strong>Is n8n a good Zapier alternative?</strong></summary>

They charge differently. n8n counts an execution as one run of the whole workflow, whatever the number of steps, while Zapier counts a task for each successful action. A workflow with many steps counts as fewer units on n8n's model, and Zapier includes its MCP server on every plan, Free included.

</details>

<details>
<summary><strong>Can these tools generate images and video?</strong></summary>

n8n's OpenAI node can generate an image, and it has app nodes for Qwen Cloud and MiniMax that generate images and video. Make documents AI steps through its AI Provider. Wireflow runs 100+ models as nodes, as [Wireflow's AI workflow orchestration page](https://www.wireflow.ai/features/ai-workflow-orchestration-platform) shows.

</details>

<details>
<summary><strong>What is n8n?</strong></summary>

n8n is a workflow automation platform that connects apps, moves data and runs AI agents. Its docs define a workflow as a collection of nodes connected together to automate a process, and its cloud plans are priced in euros by workflow executions.

</details>

## The short version

Pick Wireflow when the workflow exists to generate images, video or audio, and keep a general automation tool for the rest. Pick Zapier or Make when the job is moving data between many apps without code, and Pipedream when developers want code steps and MCP tools. Before you switch, rebuild one real n8n workflow in your two finalists and count the steps that need custom code. To start from a working board, browse [Wireflow's workflow templates](https://www.wireflow.ai/features/ai-workflow-templates).

## Contributing

Corrections and additions are welcome, including corrections to the entry for the tool that maintains this list. Open an issue with the tool name, a working link, one line on what it does that the tools already listed do not, and one line on where it stops. Entries are judged on whether they are usable today, not on popularity. Full rules in [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[CC0 1.0 Universal](LICENSE), public domain. Take the data, fork the list, no attribution required.

---

Maintained by [a1adams](https://github.com/a1adams).

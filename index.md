---
title: Home
layout: home
nav_order": 1
---

<!-- ![AI Reader](assets/general/icon.png) -->

# AI Reader

AI Reader is a free, all-in-one desktop software to help researchers and students conduct research with ease in the digital age.

{: .note }
> AI Reader is currently in the preview stage (see [development](#development)).

---

<details markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Video tutorial

### Youtube

<iframe  width="560"
        height="315"  src="https://www.youtube.com/embed/FQfvJ_zOxOE" title="AI Reader 0.1.0 Preview 90 Secs Tutorial" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Or, download the video [here](assets/v0.1.0/ai_reader_0.1.0_web_demo.mp4)

## Download

### Latest version: __{{ site.github.latest_release.tag_name }}__

Updated at: {{ site.github.latest_release.published_at | date: "%b %d, %Y" }}
{: .label .label-green }

{: .issue }
> MacOS version might have issues on older versions such as Big Sur.

[Windows]({{ site.github.latest_release.assets[1].browser_download_url }}){: .btn}
[MacOS Universal]({{ site.github.latest_release.assets[0].browser_download_url }}){: .btn}

### Past versions

Visit [releases]({{ site.github.releases_url }}) for all versions.

## Design

### Research-oriented

AI Reader focuses on the __research process__, setting it apart from other tools for reference management, note-taking,
or writing. This approach ensures it meets the unique needs of researchers.

### Multi-purpose

AI Reader is an all-in-one solution that covers the entire research cycle, from collecting materials to processing, analyzing, and finally outputting your work. This makes it a versatile tool for researchers.

### Ready-to-use

AI Reader offers a variety of tools, processors, and services with intuitive graphic interfaces. You can choose and use
these out-of-the-box features to customize your research experience.

### Local-first

Your data is stored locally on your computer in SQLite database files, which can be opened by any third-party database
applications. This ensures you're never locked into a specific platform.

### Free

AI Reader is completely free. There are no plans for an online version or a cloud service with subscription fees. The
only costs you might encounter are for services like OpenAI, which require an API account. However, even these will be
phased out as comparable free alternatives become available locally.

### By researchers, for researchers

As a fellow researcher, I understand the challenges academics face when transitioning from traditional library-based
research to a digital environment. AI Reader is designed to help you _prepare_, _read_, and _analyze_ papers in a
digital format, offering easy-to-use tools for this purpose.

At its core, AI Reader aims to eliminate repetitive manual tasks, allowing you to focus on the aspects of research that
truly matter: exploring, thinking, analyzing, and expressing. Drawing from my years of experience building tools for my
own research, I hope AI Reader continues to evolve and help others in similar situations.

## Modules

### AI Discussant (available in v0.1.0 Preview)

The first released AI Reader _module_, __AI Discussant__, allows you to chat with AI about your research materials. It
currently utilizes OpenAI's [`GPT-3.5 Turbo model`](https://platform.openai.com/docs/models/gpt-3-5) and requires an
OpenAI API key to function.

### AI Discussant Features

#### GPT Answers Tailored for Research

- AI Discussant in AI Reader focuses on academic needs, delivering thorough, sophisticated, and detailed answers backed
  by textual evidence from your document.
- Compare AI Discussant with similar products and see the difference. Feel free
  to [report issues]({{ site.github.issues_url }}) if you find AI Reader providing an inferior answer
  about the same document.

#### Consulting the Source

- AI Discussant answers include page references to the PDF document, enabling you to quickly verify and/or closely read
  the referenced page.
- Click on the provided list of keywords to search through the PDF document effortlessly.

#### Pay Only for What You Use

- ChatGPT embedding and chatting costs are estimated, so you only pay for what you use. There are no subscriptions, page
  limits, or middle-man services.

#### Index Once, Use Forever

- After indexing your document, you can not only chat with ChatGPT about it but also use the document for other
  purposes (with upcoming features) such as semantic search. There's no need to index the document again.

#### Export Chat History

- Export your chat history as a Markdown file for future reference.

### Reading Notes Organizer 

Upcoming in [v0.2.0](#roadmap)
{: .label .label-yellow }

- An integrated module that simplifies the extraction, browsing, organization, and export of your reading notes in PDF
  files.

---

## Development

### Update Cycle

AI Reader is a one-man project, and after years of exploration, it has finally reached a stage where it can
realistically support all its planned features. With most of the infrastructure (database, backend, and frontend) in
place in `v0.1.0 Preview`, new feature development will be quicker.

As a researcher rather than a full-time developer, I can't guarantee timely delivery of new modules. However, I aim for
a __monthly__ release cycle for new modules until AI Reader reaches `v1.0`. Individual features and bug fixes will be
addressed as quickly as possible in shorter update cycles.

### Modules and Features

A feature is a specific function in AI Reader, such as exporting to Markdown. A module is a collection of features
serving a broader purpose, like AI Discussant, and takes longer to develop.

### Roadmap

#### 2023

- [x] v0.1.0 Preview - AI Discussant Module - _May_
- [ ] v0.2.0 Preview - Notes Organizer Module - _June_
- [ ] More planned modules and features to be announced.

## How to Contribute

- AI Reader is free but closed-source, developed in a monorepo, and cannot accept pull requests.
- The best way to support AI Reader is
  by [reporting issues and requesting features]({{ site.github.issues_url }}) that are useful to you as
  a researcher.
- Currently, there's no option to donate to AI Reader. In the future, I may consider accepting donations for a fixed
  amount needed to obtain
  a [Microsoft EV code signing certificate](https://learn.microsoft.com/en-us/windows-hardware/drivers/dashboard/code-signing-cert-manage)
  for AI Reader. This would eliminate the security warning dialogue when running the unsigned release. However, it's
  optional for now. The Mac version is already notarized.

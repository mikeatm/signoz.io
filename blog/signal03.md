---
slug: community-update-03
title: A major release, tons of bug fixes and amazing new contributors - Signal#03
author: Pranay Prateek
author_title: SigNoz Core Team
author_url: https://github.com/pranay01
author_image_url: https://avatars.githubusercontent.com/u/504541?v=4
tags: [Product Update, Community]
---

Welcome to Signal #03 - our monthly product update!

It's that time of the month when we update our community to what we've been up to recently. This month, we left behind a trail of squashed bugs, tiny but mighty product improvements, and onboarded new contributors for our journey ahead.

We are also working on a big update on metrics ingestion for SigNoz that will massively increase the scope of performance monitoring using SigNoz. More details inside 👇

## What we shipped?

This month, we are excited to announce that our latest release had contributions from 10 awesome contributors. Release link: [v0.3.3](https://github.com/SigNoz/signoz/releases/tag/v0.3.3)

### Regex pattern matching enabled for tags

Some of our users wanted to see 4xx errors quickly. So we have enabled regex pattern matching in our trace filters. Now users can apply generic regex operations to any of their tags.
[Link to the issue](https://github.com/SigNoz/signoz/pull/249)

![You can use regex patterns for filtering traces](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8gle02ntroqigg5lpt4j.png)<figcaption>Apply regex operations on trace filters</figcaption>

### Frontend Improvements

Flamegraphs and Gantt charts make a champion combo for debugging latency issues on our dashboard. We improved the experience slightly, where selecting a trace in the flamegraph highlights the corresponding span in the Gantt chart view.

![Selecting a trace in the flamegraph highlights the corresponding span in the gantt charts](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/nmmlf68f4jdpno857k63.png)<figcaption>When you select a trace in the flamegraph, corresponding span in the Gantt chart gets highlighted</figcaption>

### Readme.md translation to Chinese

We recently conducted a [deep dive](https://signoz.io/blog/getting-to-know-our-4000-plus-stargazers-on-github/) into our stargazers and found out that the top 5 countries where our stargazers belong are from US, India, Brazil, China, and Germany.

To make our GitHub repo more accessible, we raised requests for getting our readme.md translated to different languages. [Tony Qu](https://github.com/tonyqus), a 15+ year .NET veteran, helped translate our readme.md to Chinese, and we couldn't be happier. 🤓

![Countries from which our stargazers belong](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/rzreosk921s7mmtj3ela.png)<figcaption>SigNoz's stargazers belong to nations worldwide</figcaption>

## Featured Issue

### Charts for 4xx status codes

As we mentioned earlier, users requested to visualize 4xx as errors and be highlighted in the SigNoz dashboard. Currently, we have solved it by enabling regex operations on tags. However, we would love to have your inputs on how to visualize it better. Any UI/UX suggestion is welcomed on the [issue](https://github.com/SigNoz/signoz/issues/222).

### Readme.md translations

We still have many languages to cover for our readme.md translation. If any of you can help us with [German](https://github.com/SigNoz/signoz/issues/240) or [Portugese](https://github.com/SigNoz/signoz/issues/238) translations, that would be great.

### Cypress Framework for E2E testing

Cypress is a Javascript-based end-to-end testing framework that provides users with a fast and reliable test framework. We are looking forward to implementing it as our front-end testing framework. If you have any thoughts around it, please consider commenting on the [issue](https://github.com/SigNoz/signoz/issues/226).

## What's upcoming?

### Metrics Ingestion Pipeline

With metrics ingestion pipeline, users should be able to send and visualize metrics like Dosckerstats, JMX metrics from target Mbeans server, cluster-level metrics from the Kubernetes API server, and visualize these on SigNoz UI.

This update will increase the scope of application performance monitoring manifolds. We will come out with specific tutorials on how to monitor these metrics once we launch the update.

You can find the complete list of receivers for which metrics ingestion pipeline will work [here](https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/receiver).

## SigNoz News

### Frontend Best Practices

We recently had our monthly community call. Community calls can be joined by anyone who wants to participate.

The agenda was to discuss the best practices we should follow in our frontend code, specifically around test frameworks to use, styling guides for PRs, and localization.

Some frameworks that are used in large scale companies like Uber and Verizon were suggested for our frontend development workflow:

- Jest - a Javascript testing framework
- Cypress framework - a JavaScript-based end-to-end testing framework built on top of Mocha
- RTL for component testing and integration testing

You can watch the complete call recordings here 👇

{% youtube aoOpQ3r84Dw %}

If you want to join future community calls, then you can join our [slack channel](https://bit.ly/signoz-slack). We give out all updates there.

## From our blog

Monitoring your Spring Boot application with OpenTelemetry was never this easy. OpenTelemetry provides a Java JAR agent that can be attached to any Java 8+ application. The JAR agent can detect a number of [popular libraries and frameworks](https://github.com/open-telemetry/opentelemetry-java-instrumentation/blob/main/docs/supported-libraries.md) and instrument it right out of the box. You don't need to add any code for that.

You can read the full blog here👇
[Monitor your Spring Boot application with OpenTelemetry and SigNoz](https://signoz.io/blog/opentelemetry-spring-boot/)

## Contributors

Shoutout to our new contributors [Vimal](https://github.com/Vimalraj571), [Tony](https://github.com/tonyqus), and [Rahul](https://github.com/rahulrana95), for improving SigNoz and making our community more awesome. 🥳 🎉

We also wanted to express our gratitude to [Lalit Kale](https://www.linkedin.com/in/lalitkale/) and [Rameshwar Shelge](https://www.linkedin.com/in/rameshwarshelge/) for giving active inputs around [testing](https://github.com/SigNoz/signoz/discussions/208) and strategizing [performance benchmarks for SigNoz](https://github.com/SigNoz/signoz/discussions/218).

Thank you for taking out the time to read this issue :) If you have any feedback or want any changes with the format, please create an [issue](https://github.com/SigNoz/signoz/issues).
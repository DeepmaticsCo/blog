---

layout: post  
title: "Architectural Evolution of Transformers"  
date: 2025-08-01  
image: "assets/llm-architecture/architecture.png"  
excerpt: "Exporing the architectural aspects of how decoder LLMs have imporved and code them."  
author: "Satish Yenumula"  
tags: \[GenAI, Transformers, LLM\]

---

## Introduction

As someone working on GenAI should be well versed with "Transformers architecture" and we would have gone through Jay Alammar's [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) explanation that had simplified the "Attnetion Is All You Need" paper.

In this post, we will be go beyond the basics and look at few of the major releases of decoder based large language models and look specifically into the improvements made in an LLM model's architecture. However, from a practitioner standpoint this is not usually the case, a major release that beats benchmarks has multiple aspects to it, including improvements in training data quality, LLM fine-tuning or Preference Tuning methodologies in addition to the architectural changes. However, for the scope of this post, we are only limiting to architectural improvements of a set LLMs, whose information is open-source or the technical reports have been available.

## Foundation and Early Scaling

ChatGPT by OpenAI

<table><tbody><tr><td rowspan="3"><figure class="image image-style-side"><img src="{{ site.baseurl }}\assets\llm-architecture\GPT3.png"></figure></td><td><p>GPT1</p><p>-- testing layout</p><p>In this post, we will be go beyond the basics and look at few of the major releases of decoder based large language models and look specifically into the improvements made in an LLM model's architecture. However, from a practitioner standpoint this is not usually the case, a major release that beats benchmarks has multiple aspects to it, including improvements in training data quality, LLM fine-tuning or Preference Tuning methodologies in addition to the architectural changes. However, for the scope of this post, we are only limiting to architectural improvements of a set LLMs, whose information is open-source or the technical reports have been available.</p><p>&nbsp;</p></td></tr><tr><td>GPT2</td></tr><tr><td>GPT3</td></tr><tr><td colspan="2">Code Repo Link</td></tr></tbody></table>